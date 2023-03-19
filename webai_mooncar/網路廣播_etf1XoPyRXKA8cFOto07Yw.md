 

# 網路廣播

Web:AI 的網路廣播功能，不僅能讓 Web:AI 與 Web:AI 開發板彼此資訊互動，更可以和 Webduino 的其它平台之間連動。實現一對多、多對一、虛實互動、遠距廣播...等多樣化的操控情境，透過廣播功能的實現，便能將物聯網的應用發揮到極致。

> 有關 Web:Bit 教育版的積木操作，可以參考：[Web:Bit 教學手冊](https://webbit.webduino.io/tutorials/doc/zh-tw/education/index.html)

## 發送廣播訊息

「發送廣播訊息」積木可以指定一個頻道名稱，並對這個頻道發送訊息文字，只要頻道名稱相同，所有在該頻道上的裝置都能收到廣播訊息。不論是實體裝置、虛擬裝置、沒有開發板的程式...等，都能夠向指定頻道發送廣播訊息。

> 執行程式時遇到「發送廣播訊息」積木會暫停，直到發送廣播訊息後才會再繼續。

<img src="https://md.webduino.io/uploads/upload_c88532e5120c700bfcf05e60f04c99b1.png" alt="" width="">

### 範例：向 Web:Bit 教育版發送訊息

1. 使用「發送廣播訊息」積木，設定向「channel」頻道傳送訊息「Hello!」，按下執行。

   <img src="https://md.webduino.io/uploads/upload_8650137f8c6e3a009d5ce1653ebdac9d.png" alt="" width="">

2. 開啟 [Web:Bit 教育版](./Web_Bit 教育版_blockly.md)
3. 放入「接收廣播訊息」積木，設定從頻道「channel」接收廣播訊息。
4. 放入「綠色怪獸說話」積木讓舞台中的小怪獸說出廣播訊息。
5. 按下執行，可以看到小怪獸舞台的小怪獸說出來自 Web:AI 發送的訊息。

>- Web:Bit 教育版的網路廣播積木位在 **擴充功能 > 網路廣播**。
>- Web:Bit 教育版的小怪獸說話積木位在 **進階功能 > 怪獸控制**。

<img src="https://md.webduino.io/uploads/upload_09e5eb963c47a4f78acb13c615351799.png" alt="" width="">

## 接收廣播訊息

「接收廣播訊息」積木可以指定一個頻道名稱，不斷收聽這個頻道的變化，並透過廣播訊息的積木顯示。接收廣播訊息不限制只有實體裝置能接收，不論是實體裝置、虛擬裝置、沒有開發板的程式...等，都能夠接收指定頻道的訊息。

> 「接收廣播訊息」積木不需要放在重複迴圈內，就會自行不斷收聽頻道訊息。

<img src="https://md.webduino.io/uploads/upload_3866a2c19e7bf44bb6226584cd4503c9.png" alt="" width="">

### 範例：接受來自 Web:Bit 教育版的訊息

1. 開啟 [Web:Bit 教育版](./Web_Bit 教育版_blockly.md)
2. 使用「發送廣播訊息」積木，設定向「channel」頻道傳送訊息「Hello!」，按下執行。

   <img src="https://md.webduino.io/uploads/upload_77702faa143913ce68f8d197e0a82b12.png" alt="" width="">

3. 打開 Web:AI 程式積木平台。
4. 使用「接收廣播訊息」積木，設定從「channel」接收廣播訊息。
5. 放入「LCD 顯示文字」積木顯示「收到的廣播訊息」。
6. 按下執行，可以看到 Web:AI 開發板螢幕顯示廣播訊息「Hello!」

   <img src="https://md.webduino.io/uploads/upload_9ec090d270752bd264fa827568388471.png" alt="" width="">

