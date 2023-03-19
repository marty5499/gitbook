---
title: 人臉辨識教學 - Web:AI 教學手冊
description: Web:AI 人臉辨識可以透過最簡單的方式學習人臉辨識原理，透過程式積木組合，自行編寫門禁系統、上班打卡、人臉解鎖等等人臉辨識應用功能，體驗最熱門的 AI 教育應用。
GA: UA-62202920-22 
---

 

# 人臉辨識

在 AI 科技教育中，常見的人臉辨識能夠根據人臉的特徵，如：眼睛、鼻子、嘴巴等，計算出人臉的特徵值。再藉由比對各個人臉的特徵值，判斷人臉的身份以及相似度。

Web:AI 除了可以學習人臉辨識原理，還能提供人臉的座標位置、辨識信心度，在課堂中做出輕鬆人臉辨識、門禁系統、照片比對、人臉解鎖等等 AI 生活應用。

## 匯入人臉模型

在使用「人臉辨識」積木前，需要先透過「匯入模型」將「人臉辨識模型」下載入板子中，才能開始進行人臉辨識。

### 步驟

1. 下載[人臉辨識模型](https://drive.google.com/uc?export=download&id=1zPPtIxObstJ4yNCF80_vqF0onZDc7Q5J)

    <img src="https://md.webduino.io/uploads/upload_9d610624bcffc082787e375c5c3ae3f1.png" alt="" width="">

2. 將 Web:AI 開發板透過 USB 連接上積木平台。

2. 點擊「更多」中的「匯入模型」。

    <img src="https://md.webduino.io/uploads/upload_3d6e7a11528d4610e64b55ab4491b1b1.png" alt="" width="">

3. 選擇剛剛下載的「face_recognition.kmodel」。

4. 等待匯入模型完成就可以開始使用「人臉辨識」積木！

    <img src="https://md.webduino.io/uploads/upload_90bbbddcc7d9b277cace0f2286e5b7a5.png" alt="" width="">

## 開始人臉辨識

「開始人臉辨識」積木會自動開啟 Web:AI 開發板鏡頭，並讀取人臉辨識模型。
使用時，可以透過右側方框選擇：
- 是否框選螢幕中的人臉
- 是否框選螢幕中的人臉五官

<img src="https://md.webduino.io/uploads/upload_4ecd716f096be04c1b695fcd8288c87f.png" alt="" width="">

使用時會**執行辨識 1 次**，可以搭配「重複」積木重複辨識。

<img src="https://md.webduino.io/uploads/upload_3fd1adec15a039de3d4712d5302b8aec.png" alt="" width="">

## 人臉特徵值

在比對人臉前，需要先取得人臉的特徵值，「人臉特徵值」積木能夠將人臉五官特徵轉換成字串資訊。
藉由比對這些「人臉特徵值」，能夠判斷人臉之間的相似度。

<img src="https://md.webduino.io/uploads/upload_6ef736b9a7f1a3c1e6f4f9abd25c0f36.png" alt="" width="">

將「拍攝照片」積木或「圖檔」積木放入，能夠將拍攝到的照片或圖檔中的人臉資訊轉換成特徵值。

<img src="https://md.webduino.io/uploads/upload_22c21ccf1909577d1d3d9dbbad0848ec.png" alt="" width="">

> 因為使用的模型與訓練方式不同，無法和 [Webduino 兌換券 - 人臉辨識＋情緒感知](https://store.webduino.io/products/voucher-face) 中的臉部特徵值共用！

### 範例：說出人臉的特徵值

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用「開始人臉辨識」積木搭配「重複」積木，讓 Web:AI 能不斷辨識人臉。

    <img src="https://md.webduino.io/uploads/upload_079903252ec3f1ae0736968afb56cdd8.png" alt="" width="">

2. 將「拍攝照片」積木放入「人臉特徵值」積木中，並使用「按鈕」積木觸發動作。

    <img src="https://md.webduino.io/uploads/upload_625f45bc493e31b28e14d032f767da8c.png" alt="" width="">

3. 完成積木如下，執行後對著拍攝的人臉按下 L 按鈕，可以看到小怪獸說出特徵值。

    > 特徵值為一段相當長的字串。

    <img src="https://md.webduino.io/uploads/upload_020461221299149c009044a7051c48ec.png" alt="" width="">


    <img src="https://md.webduino.io/uploads/upload_d6856b6a9f3000e05e040ce07d99da14.png" alt="" width="">

## 人臉命名

為了做出門禁系統等生活應用情境，需要將「取得的特徵值」紀錄到 Web:AI 中，「人臉命名」積木能夠將人臉命名為「小明」、「小王」等自訂的名稱。

> 因為人臉數量越多會影響辨識度，建議設定人臉數量為 5 個內。

<img src="https://md.webduino.io/uploads/upload_34004d852e8f6f2e3bf7d524428630da.png" alt="" width="">

「人臉命名」積木中必須放入「人臉特徵值」積木。

<img src="https://md.webduino.io/uploads/upload_cf67921f641b0d353855e27db29b890c.png" alt="" width="">

## 人臉資訊

辨識到人臉時，可以使用「人臉資訊」積木取得以下資訊：
- 名稱 
- 信心度
- x 座標
- y 座標

<img src="https://md.webduino.io/uploads/upload_56dc3641abfda6b1fe4c320f5317d797.png" alt="" width="">

人臉名稱為「人臉命名」積木設定的人臉

> 如果辨識到的是未設定的人臉，則會顯示半形問號「?」。

<img src="https://md.webduino.io/uploads/upload_ef85d1a585754d0288589b4ea6d6cffe.png" alt="" width="">

### 範例：辨識與設定人臉

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用「開始人臉辨識」積木，搭配「LCD 顯示」積木和「重複」積木，能夠重複辨識並在螢幕上顯示人臉名稱。

    <img src="https://md.webduino.io/uploads/upload_5eb20fd4703e6087043845b7b7af2c58.png" alt="" width="">


2. 在程式剛執行時，設定變數「順序」為 0，並在每次按下 L 按鈕時「順序」增加 1。

    <img src="https://md.webduino.io/uploads/upload_ce8423b79d3cfa46070fa11192912b07.png" alt="" width="">

3. 接著分別設定 ( 此處命名的字串可以自訂名稱 )：
    - 當順序 = 1：將拍攝的人臉命名為「studentA」
    - 當順序 = 2：將拍攝的人臉命名為「studentB」
    - 當順序 = 3：將拍攝的人臉命名為「studentC」

    <img src="https://md.webduino.io/uploads/upload_fd0052117aa94207ead747e915bba5cc.png" alt="" width="">

4. 將積木組合起來如下圖，按 L 按鈕分別設定人臉 A、B、C，並且在螢幕上顯示辨識到的人臉名稱。

    <img src="https://md.webduino.io/uploads/upload_299552a134a804739d5ed3a241102811.png" alt="" width="">

## 應用範例：LINE 警報通知

#### ➤ 前往 [`範例連結`](https://ai-blockly.webduino.io/?hashid=gM0MeleZAN#/)

當 Web:AI 偵測到不認識的人臉時，會傳送照片連結和警報訊息到 LINE。

1. 使用「開始人臉辨識」積木，搭配「重複」積木，能夠重複辨識螢幕上的人臉。

    <img src="https://md.webduino.io/uploads/upload_fb1b5c44c3484a7081755d70c3608b6d.png" alt="" width="">

2. 辨識到陌生人會發送通知。
使用「邏輯」積木搭配「重複」積木，當「辨識人臉的名稱」是「?」時，會執行後續的動作。
因為使用到兩個「重複」積木，所以需要勾選「背景執行」。

    <img src="https://md.webduino.io/uploads/upload_764b1ab902a727ab425cc3254ae8973a.png" alt="" width="">

3. 先拍照上傳雲端，再將圖片網址透過 LINE Notify 發送，加入 2 秒的延遲時間。
    >- 使用前必須先設定 LINE Notify，歡迎參考：[LINE 積木](./LINE 積木_bi0d3z5CRgqMXJIvcks6-g.md)。
    >- 因為「重複」積木會不斷發送訊息，因此多增加 2 秒的時間間隔。

    <img src="https://md.webduino.io/uploads/upload_61593802e2bd1327376cf3fc6df8c78a.png" alt="" width="">

4. 將積木組合如下，當辨識到陌生人時，會傳送照片連結並發送 LINE 通知。

    <img src="https://md.webduino.io/uploads/upload_2ad76690edaf5f61cc0c8d5ec5fa2972.png" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_62039cbefa603da7899a0a41cf9182fb.png" alt="" width="">
