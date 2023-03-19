#### tags: `micropython` > [[回首頁]](https://md.webduino.io/cYuxdDkOSJ2guIzPG-KHqA?view)

Esp32Cam
====
> [[回首頁]](https://md.webduino.io/cYuxdDkOSJ2guIzPG-KHqA?view)

<img src="https://md.webduino.io/uploads/upload_613552a6581a20069bbb7f60dfd4aa2e.png" alt="" width="">


### 內建一顆LED燈 GPIO33
<img src="https://md.webduino.io/uploads/upload_ebaba600efb4e1d24ee751bf582bcdcc.png" alt="" width="50%">

## MicroSD 使用腳位
The following pins are used to interface with the microSD card when it is on operation.


| MicroSD            |   ESP32 | 可用 |
|:------------------ | -------:| ----:|
| CLK                |  GPIO14 |    ✔ |
| CMD                | GPIO 15 |    ✔ |
| DATA0              |  GPIO 2 |    ✔ |
| DATA1 / flashlight |  GPIO 4 |      |
| DATA2              | GPIO 12 |      |
| DATA3              | GPIO 13 |    ✔ |

| 其他腳位  |   ESP32 | 可用 |
|:--------- | -------:| ----:|
| Uart0 TXD |  GPIO 1 |    ✔ |
| Uart0 RXD |  GPIO 3 |    ✔ |
| Uart2 RXD | GPIO 16 |    ✔ |


## 鏡頭

X-JM0007A 廣角鏡頭
<img src="https://md.webduino.io/uploads/upload_c9d99f62e9f5bc3fc87226496ab3d8bd.png" alt="" width="">

X-JM0008B 魚眼鏡頭
<img src="https://md.webduino.io/uploads/upload_8a2748cbd0b43302575d945729da2548.png" alt="" width="">

## Touch Enable
There are ten capacitive touch-enabled pins that can be used on the ESP32: 
0, 2, 4, 12, 13 14, 15, 27, 32, 33

## ADC
- ADC1:
    - 8 channels: GPIO32 - GPIO39

- ADC2:
    - 10 channels: GPIO0, GPIO2, GPIO4, GPIO12 - GPIO15, GOIO25 - GPIO27

## 編譯 esp32-cam 韌體 (esp-idf v4.2)

### 1.準備好相關套件與環境設定
```console=
mdir ~/esp32-mpy
cd ~/esp32-mpy

# clone micropython repo
git clone https://github.com/micropython/micropython.git

# clone 開發者 lemariva's repo
git clone https://github.com/lemariva/micropython-camera-driver

# 使用 Docker's esp-idf 環境，掛入當下 micropython 目錄
docker run --rm -v $PWD:/project -w /project -it espressif/idf:release-v4.2

# 到 esp-idf 元件目錄下，新增 esp32-cam 元件
cd /opt/esp/idf/components
git clone https://github.com/espressif/esp32-camera

# 切換到這個點，這是試過可以編譯成功的點
cd esp32-camera
git checkout 221d24da1901b6aee8df6c1a1160ad02faa685b5
# 新版本
git checkout 093688e0b3521ac982bc3d38bbf92059d97e3613

# COPY esp32cam 開發板建置參數的相關目錄
cd /project/micropython/ports/esp32
cp -R ../../../micropython-camera-driver/boards/* /project/micropython/ports/esp32/boards/
```

:::danger
最特殊的一步，修改 main.c，找到關鍵字進行註解
:::
```c=
main.c: modify the lines inside the #if CONFIG_ESP32_SPIRAM_SUPPORT || CONFIG_SPIRAM_SUPPORT, they should look like:
    /*
    // Try to use the entire external SPIRAM directly for the heap
    size_t mp_task_heap_size;
    void *mp_task_heap = (void *)SOC_EXTRAM_DATA_LOW;
    switch (esp_spiram_get_chip_size()) {
        case ESP_SPIRAM_SIZE_16MBITS:
            mp_task_heap_size = 2 * 1024 * 1024;
            break;
        case ESP_SPIRAM_SIZE_32MBITS:
        case ESP_SPIRAM_SIZE_64MBITS:
            mp_task_heap_size = 4 * 1024 * 1024;
            break;
        default:
            // No SPIRAM, fallback to normal allocation
            mp_task_heap_size = heap_caps_get_largest_free_block(MALLOC_CAP_8BIT);
            mp_task_heap = malloc(mp_task_heap_size);
            break;
    }
    */
    size_t mp_task_heap_size;
    mp_task_heap_size = 2 * 1024 * 1024;
    void *mp_task_heap = malloc(mp_task_heap_size);
    ESP_LOGI("main", "Allocated %dK for micropython heap at %p", mp_task_heap_size/1024, mp_task_heap);
```

### 2.編譯 esp32Cam 韌體

```console=
# 然後到 micropython 目錄建置 cross
cd /project/micropython
make -C mpy-cross


# 終於可以編譯 ESP32CAM 韌體了
cd /project/micropython/ports/esp32

make USER_C_MODULES=../../../../micropython-camera-driver/src/micropython.cmake  BOARD=GENERIC_CAM all

# 新版本改用 ESP32_CAM
make USER_C_MODULES=../../../../micropython-camera-driver/src/micropython.cmake BOARD=ESP32_CAM all

```

### 3.燒錄 esp32Cam 韌體 (使用 esptool.py 燒錄)
:::danger
燒錄不在容器內，並且需使用conda切換運行環境
conda activate esp32
:::

```console=
## 進入產生韌體的目錄
cd ~/esp32-mpy/micropython/ports/esp32/build-GENERIC_CAM

## erase flash
esptool.py -p /dev/cu.usbserial-1440 erase_flash

## 燒錄韌體
esptool.py -b 230400 -p /dev/cu.usbserial-1440 write_flash 0x8000 partition_table/partition-table.bin 0x1000 bootloader/bootloader.bin 0x10000 micropython.bin
```



