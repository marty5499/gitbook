#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md) / [`Web:AI MoonCar`](./`Web_AI MoonCar`_WL73SmMMQN-Aw217YB_Z3g.md)

# 交通號誌辨識 ( 附模型下載 )

在 Web:AI MoonCar 中，附贈了 9 張交通號誌卡（手邊沒有小卡可到 [這裡](https://pse.is/4ltbv2) 下載列印），能夠使用 Web:AI 的物件追蹤功能，讓小車可以自動偵測交通號誌，並做出對應的行動。

看到「慢」號誌會降低速度，看到「喇叭」號誌會透過喇叭發出音檔，除此之外有更多更多自駕車的應用情境，都可以透過 Web:AI MoonCar 及程式積木做出來。

<img src="https://md.webduino.io/uploads/upload_869483906f59ce896836c4676d9c2ec2.png" alt="" width="">

<br>
<br>
<br>

## 一、下載交通號誌模型

在做交通號誌辨識前，需要先將「交通號誌模型」下載入板子中，可以透過「 A. USB 匯入模型」或是透過「 B. 影像訓練平台」。

> 選擇 A 或 B 其中一種方式匯入模型。 

### A. USB 匯入模型 

1. 下載[交通號誌模型](https://drive.google.com/uc?export=download&id=1ysH_sj4gG5UA9jq6V7ge9NMaPgdASSGf)。

    <img src="https://md.webduino.io/uploads/upload_788902840cbcbbe49223354e8ca774e1.png" alt="" width="">

3. 點擊「更多」中的「匯入模型」。

    <img src="https://md.webduino.io/uploads/upload_07d1a246adb87d1e684c519ec7b4798f.png" alt="" width="">

4. 將 Web:AI 透過 USB 連上積木平台，選擇剛剛下載的「model.kmodel」。

5. 等待匯入模型完成就可以開始使用「交通號誌積木」！

    <img src="https://md.webduino.io/uploads/upload_13bdd68b5efdefc51d9e2bd1582bb2b1.png" alt="" width="">

### B. 影像訓練平台下載交通號誌模型

1. 前往 [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md)。
2. 點擊「模型」。

    <img src="https://md.webduino.io/uploads/upload_af14751e7941896c3849ee42cc3cec44.png" alt="" width="">

3. 點擊「新增」，出現「新增模型」畫面。

    <img src="https://md.webduino.io/uploads/upload_1de06395cb22454df52b67e0c0b2439c.png" alt="" width="">

4. 設定模型：

    - 輸入「模型名稱」
    - 選擇種類為「物件追蹤」
    - 點擊「複製公開模型」

5. 搜尋「TrafficSigns」模型，勾選後點擊「建立模型」。

    > 大小寫都可以搜尋。

    <img src="https://md.webduino.io/uploads/upload_579722248a398d2e0c8461e375916e80.png" alt="" width="">

6. 等待訓練完成後，就可以在模型列表中看到訓練好的交通號誌模型。

    <img src="https://md.webduino.io/uploads/upload_d93571a04f6d2f296e86678eaefcef7c.png" alt="" width="">

7. 點擊「交通號誌模型」，選擇「下載模型」後輸入 Web:AI 的 Device ID，並開始下載。

8. 模型下載完成就可以開始使用「交通號誌積木」！

<br>
<br>
<br>

## 二、辨識交通號誌積木

### <img src="https://md.webduino.io/uploads/upload_6d015784134ff6c124bc40516ffdca9a.png" alt="" width=""> 開始辨識交通號誌

使用「開始辨識交通號誌」積木會自動開啟鏡頭並讀取交通號誌模型，當辨識到號誌時會將螢幕上的號誌框起來。

<img src="https://md.webduino.io/uploads/upload_15b37e6bdc0516de69b910636ebadae3.png" alt="" width="">

使用時會**執行辨識 1 次**，可以搭配「重複」積木重複辨識。

<img src="https://md.webduino.io/uploads/upload_2c0f02a97a7ccdf1d1d00fb16aa62e1f.png" alt="" width="">

### <img src="https://md.webduino.io/uploads/upload_6d015784134ff6c124bc40516ffdca9a.png" alt="" width=""> 如果辨識到號誌執行

「如果辨識到號誌執行」積木用法類似「如果執行」積木，當辨識到指定的號誌時，會做出後續的程式。

<img src="https://md.webduino.io/uploads/upload_10383518800a04e354e52a206c84d38c.png" alt="" width="">

### <img src="https://md.webduino.io/uploads/upload_6d015784134ff6c124bc40516ffdca9a.png" alt="" width=""> 號誌的資訊

「號誌的資訊」積木能夠取得偵測到號誌的資訊，有：
- x 座標
- y 座標
- 寬
- 高
- 信心度

<img src="https://md.webduino.io/uploads/upload_d7f77d18b40fedcba03bede2de099df4.png" alt="" width="">

搭配「邏輯」積木做使用。

<img src="https://md.webduino.io/uploads/upload_451debf91232a0b0711ff3c65e9477b8.png" alt="" width="">

<br>
<br>
<br>

## 三、範例：按喇叭

1. 先下載交通號誌模型。
2. 使用「開始辨識交通號誌」積木加上「無限重複」積木，讓 Web:AI 開始辨識交通號誌。

    <img src="https://md.webduino.io/uploads/upload_c9cdb2f7da0d5889e8658e4a4feacd10.png" alt="" width="">

3. 加入「如果辨識到號誌執行」積木，選擇「按喇叭」。

    <img src="https://md.webduino.io/uploads/upload_159af20b36229dfd0fdb2ed5120cc900.png" alt="" width="">

4. 加入「蜂鳴器」積木。
執行後，當辨識到「按喇叭」號誌時，MoonCar 會發出聲音。

    <img src="https://md.webduino.io/uploads/upload_922de012ce7032843e9946911956dccf.png" alt="" width="">

5. 如果要讓辨識更準確，可以加入「號誌的資訊」積木，數值可以根據現場狀況調整。
執行後，當「按喇叭」號誌寬度 > 30 時，MoonCar 會發出聲音。

    <img src="https://md.webduino.io/uploads/upload_8352e7b26543f90ab1c9165e36d71963.png" alt="" width="">

<br>
<br>
<br>

## 四、範例：循跡 + 辨識開頭燈

1. 先下載交通號誌模型。
2. 貼上黑色膠帶作為軌道。
4. 放入「循跡」積木及「開始辨識交通號誌」積木。

    <img src="https://md.webduino.io/uploads/upload_8fa04ca0a26efca80aea84c16eba09c6.png" alt="" width="">

3. 放入「如果辨識到號誌執行」積木，選擇「開亮頭燈」。

    <img src="https://md.webduino.io/uploads/upload_97581ff72e9b141f2dcd333b61a5a8bb.png" alt="" width="">

4. 放入 4 塊「魔幻 LED」積木，分別設定：
    - 第：1、2、3、4 顆
    - 顏色：白色

    <img src="https://md.webduino.io/uploads/upload_f242f3a06c7abef27b749c8f702bb395.png" alt="" width="">

5. 加入「關閉魔幻 LED」積木，讓沒辨識的「開亮頭燈」時，會關閉魔幻 LED。

    <img src="https://md.webduino.io/uploads/upload_82acadb79056552d4a6abf34a6e7a71a.png" alt="" width="">

6. 按下執行，MoonCar 會在軌道上行駛，並在偵測到「開亮頭燈」
