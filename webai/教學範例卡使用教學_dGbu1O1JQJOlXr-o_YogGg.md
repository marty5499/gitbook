#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md)

# 教學範例卡使用教學

教學範例卡是 Web:AI 為了各教育單位提供的程式範例，只要使用開發板掃描 QRcode，就能立即體驗 AI 人工智慧，並快速在課堂中演示範例。

## 教學影片

歡迎參考下方教學影片：

<iframe src="https://www.youtube.com/embed/Qgtthh7d9xQ" allowfullscreen width="100%" style="aspect-ratio:728/410;border:none " ></iframe>

## 介紹

教學範例包含：

A. 人臉追蹤
B. 語音互動
C. 小怪獸追蹤
D. 口罩偵測
E. 登月小車追蹤小怪獸
F. 萬用遙控器控制登月小車

> 「登月小車追蹤小怪獸」及「萬用遙控器控制登月小車」範例需要搭配登月小車作使用。歡迎參考：[MoonCar 登月小車](https://store.webduino.io/products/webbit-mooncar)。

<img src="https://md.webduino.io/uploads/upload_86e43decc1a7d68c02e3d29b8afa6486.png" alt="" width="">

## 使用教學

1. 使用 Web:AI 開發板進入 QRcode 模式
 
   > 關於如何進入 QRcode 模式，歡迎參考：[操作模式：QRcode 模式教學](https://md.webduino.ioundefined)。

2. 拿出教學範例卡，翻到背面的 QRcode。

   <img src="https://md.webduino.io/uploads/upload_c79aff377c0b1565abb23ab50cdf9a90.png" alt="" width="">

3. 使用 Web:AI 開發板的鏡頭掃描卡片上的 QRcode。

   <img src="https://md.webduino.io/uploads/upload_b472c160f3232af5abd5b0eaadc6132c.png" alt="" width="">

5. 掃描成功後即可使用教學範例！

## A. 人臉追蹤

以人臉的五官來作為模型，經過機器學習後可以追蹤出畫面中的人臉。
不限定人臉數量、會受到環境光線影響。

<img src="https://md.webduino.io/uploads/upload_fc87a0d0fbc684b427ac1f6884f322fe.png" alt="" width="">

>- 關於人臉追蹤，歡迎參考：[人臉追蹤積木](./人臉追蹤積木_cBj7ES-URbiZFz_dRR7K5Q.md)。

## B. 語音互動

基於「語音辨識」的原理實現的語音互動，開發板中放入了男性、女性、Google 小姐等語音，偵測到聲音頻率變化而做出對應的效果。使用前需要裝設喇叭。

<img src="https://md.webduino.io/uploads/upload_a963ed1f635edc162946092166344927.png" alt="" width="">

包含 3 種不同互動，只要對著 Web:AI 說出「你好嗎？」、「自拍」、「你是誰？」，就會做出不同的互動效果

> 因為每個人的聲音模型都不同，如果偵測不靈敏，可以使用 Google 小姐來說出指令。

### 1. 你好嗎？

LCD 螢幕隨機顯示 1 隻小怪獸及情緒，並透過麥克風發出對應的音效。

### 2. 自拍

Web:AI 開發板開啟攝像鏡頭，對著自己拍一張照片並顯示在 LCD 螢幕上。

### 3. 你是誰？

夢想成為科技教具的 Web:AI 會自我介紹給大家聽！

>- 關於語音辨識，歡迎參考：[語音辨識積木](./語音辨識積木_gROLWXjjSAWQCSvRzKlUMg.md)。

## C. 小怪獸追蹤

採用「物件追蹤」的技術辨識並追蹤 4 隻小怪獸，根據畫面中的小怪獸顯示資訊。

<img src="https://md.webduino.io/uploads/upload_2964da9e487533253728e42b692106fd.png" alt="" width="">

>- 關於物件追蹤，歡迎參考：[四、訓練影像分類、物件追蹤](./四、訓練影像分類、物件追蹤_4LZCe8DqSP6T0c0KPnbJPQ.md)。
>- 關於回復韌體，歡迎參考：[Web:AI 開發板基礎設定（初次使用開發板看這裡）](./Web_AI 開發板基礎設定（初次使用開發板看這裡）_ZjV1vnESTg6uZOXC77aP8w.md)。

## D. 口罩偵測

配合疫情時事，以人臉模型和配戴口罩的人臉模型做出的口罩偵測。

- 當偵測到人臉配戴口罩，顯示「安全！」。
- 當偵測到人臉**未**配戴口罩，顯示「危險！」。

<img src="https://md.webduino.io/uploads/upload_49f5f3bf9c0c9758d2afc71cdbbbd849.png" alt="" width="">

>- 關於口罩偵測，歡迎參考：[人臉追蹤積木](./人臉追蹤積木_cBj7ES-URbiZFz_dRR7K5Q.md)。

## E. 登月小車追蹤小怪獸

登月小車結合「物件追蹤」技術，辨識 4 隻顏色的小怪獸，讓魔幻 LED 發出相對應顏色的光，並且依據 LCD 螢幕中小怪獸的位置來控制登月小車的前進、左轉、右轉，讓小車追著小怪獸行駛。

<img src="https://md.webduino.io/uploads/upload_a53a4388615c70d2dff2596ed0c7350b.png" alt="" width="">

## F. 萬用遙控器控制登月小車

想要直接操控登月小車嗎？
「 Webduino 萬用遙控器」可以直接滑動網頁中的小車圖案，用最簡單的方式控制小車的移動。

<img src="https://md.webduino.io/uploads/upload_4ec04f8ec8a7eed76cda49db003b6e3c.png" alt="" width="">

### 操作步驟

1. 使用 Web:AI 開發板掃描「萬用遙控器控制小車 QRcode 」,進入「萬用遙控器控制小車」模式。
進入後可以看到螢幕顯示 QRcode 及「請用手機掃描」。

   <img src="https://md.webduino.io/uploads/upload_18b796b949623c844f4c3c82e4f33546.png" alt="" width="">

2. 使用手機掃描螢幕上的 QRcode,進入 Webduino 萬用遙控器介面。
( 也可以直接點擊 [Webduino 萬用遙控器](https://webduinoio.github.io/webduino-remote/index.html) 連結進入 )

   <img src="https://md.webduino.io/uploads/upload_16b89d4576479a4cb74d65eff5f5ec3c.png" alt="" width="">

3. 點擊右上角選單按鈕,開啟設定畫面。

    <img src="https://md.webduino.io/uploads/upload_65a2c6e74428129cd5c55c8c4ba1c9ea.png" alt="" width="">

4. 在「發送」欄位輸入 **DeviceID/PING**。
   ( 如：DeviceID 為 **1a23b4**，則是輸入 **1a23b4/PING** )

    <img src="https://md.webduino.io/uploads/upload_ccc8072293fc841a1176e178dbb53206.png" alt="" width="">


5. 輸入完畢後，點擊右上角 ✕ 符號關閉,即可滑動中央的小車圖案來操控小車移動。

   <img src="https://md.webduino.io/uploads/upload_40883633de2dcda3b46109841967b441.gif" alt="" width="">

> 如果 iOS 無法使用，歡迎參考：[常見問題：iOS 無法使用萬用遙控器怎麼辦？](https://md.webduino.io/8wr6O1G8SiuHwnopoums3w?view#%E4%BD%BF%E7%94%A8%E5%95%8F%E9%A1%8C)
