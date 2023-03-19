 

# 偵測

在「偵測」積木中，包含了鍵盤、時間、對話框等偵測方式，透過這些就可以達到用不同裝置觸發程式的功能。

## 鍵盤偵測

「鍵盤偵測」積木可以偵測電腦鍵盤的按鍵動作，根據偵測這些不同的動作來觸發不同的程式，包含以下兩種行為：

- 按下
- 放開

<img src="https://md.webduino.io/uploads/upload_a5b2a4f9bbdf2524336935427800ba92.jpg" alt="" width="">

搭配「網頁互動區域：鍵盤控制」可以達到更多物聯網遠端控制的效果。

> 偵測鍵盤行為積木處於隨時偵測的狀態，不需要搭配無限重複迴圈！

### 網頁互動區域：鍵盤控制

<!-- Web:AI 積木平台中提供了網頁互動區域，根據程式設計將執行結果顯示在網頁上，可以讓開發板達到遠端控制。 -->

透過網頁及開發板的訊息傳輸，可以將目前按下的鍵盤按鍵顯示在網頁中。

可以看到當按下鍵盤的「A」鍵，網頁互動區會馬上顯示「A」。

<img src="https://md.webduino.io/uploads/upload_6371d4c02ff60c837f2b2ce55d45674c.gif" alt="" width="">

### 範例：按鍵控制

1. 使用「鍵盤偵測」積木，選擇當鍵盤「按下」「A」鍵。

    <img src="https://md.webduino.io/uploads/upload_b4d60764f110dccd202fb4535010393b.jpg" alt="" width="">

2. 放入「小怪獸說話」積木，輸入要讓小怪獸說的話。

    <img src="https://md.webduino.io/uploads/upload_9aec82568e54c03817e519e1c9b01bb1.jpg" alt="" width="">

3. 開啟網頁互動區，按下執行。

    <img src="https://md.webduino.io/uploads/upload_63cb78e6ed722bef65ef75dfb66ff46a.jpg" alt="" width="">


4. 積木部署後按下電腦的「A」按鍵，可以看到網頁互動區的小怪獸說：「Hello」。

    <img src="https://md.webduino.io/uploads/upload_7bf91964ba2e3ffaf4c3cd12c83b2d12.jpg" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_5e8d3a177e5ac75c844c677b89b861d0.jpg" alt="" width="">

### 範例：移動白球

透過點擊小怪獸傳輸指令，改變 LCD 螢幕中白球的位置。

1. 建立「函式」，放入「清除 LCD 畫面」積木及「LCD 畫圓」積木作為白球，
並用「變數 x」、「變數 y」作為白球的座標。

   <img src="https://md.webduino.io/uploads/upload_1292fbd63c44c7789a12cc932bcb7662.jpg" alt="" width="">

2. 設定 x、y 的初始值。

   <img src="https://md.webduino.io/uploads/upload_2a5c6daf7fa5dd214f8305a8db622884.jpg" alt="" width="">

3. 放入「鍵盤偵測」積木，當按下上下左右時，改變白球 x、y 的數值。

   <img src="https://md.webduino.io/uploads/upload_33fe952a4e46b9d70b9734b8b9504ca0.jpg" alt="" width="">

4. 放入「函式」積木，當觸發動作時，會改變白球 x、y 的數值。
 
   <img src="https://md.webduino.io/uploads/upload_f1a1c096f9d4494e667d135bb18752ac.jpg" alt="" width="">

5. 完成程式如下，開啟「網頁互動區域」並按下執行，可以看到畫面如下。

    <img src="https://md.webduino.io/uploads/upload_9cec5c1b653fe557f27935ab733760bc.jpg" alt="" width="">

6. 按下鍵盤上下左右，可以控制開發板螢幕上白球的往四個方向移動。

## 對話框

「對話框」積木可以透過網頁互動區的對話框輸入文字，根據偵測這些輸入文字來觸發後續的程式。

### 在對話框輸入文字

「在對話框輸入文字」積木可以偵測輸入的文字 **1 次**。
程式執行時遇到這塊積木會暫停，直到輸入文字後才會再繼續。

<img src="https://md.webduino.io/uploads/upload_0ddc80a6f0afcb9ee363f710b6bec297.jpg" alt="" width="">

如果需要重複使用對話框，就需要在外層放入「重複積木」。

<img src="https://md.webduino.io/uploads/upload_01c426eb3f12e711a78da7a2b2c2b3eb.jpg" alt="" width="">

### 輸入的文字

「輸入的文字」積木必須放在「對話框輸入文字」積木之後，使用時會取得從對話框輸入的文字。

<img src="https://md.webduino.io/uploads/upload_5639008eb3497f88b701ec0af1bef94e.jpg" alt="" width="">

### 範例：輸入文字讓小怪獸說話

1. 使用「無限重複」積木，放入「在對話框輸入文字」積木，讓對話框可以重複使用。

    <img src="https://md.webduino.io/uploads/upload_376436ce9059d5b5819194f162b281f7.jpg" alt="" width="">

2. 組合「小怪獸說話」積木和「輸入文字」積木，讓小怪獸可以說出輸入的文字。

    <img src="https://md.webduino.io/uploads/upload_5973d53c53ffc16b2bb814f7575e1e0a.jpg" alt="" width="">

3. 打開網頁互動區，互動方式選擇「對話框」。

    <img src="https://md.webduino.io/uploads/upload_63cb78e6ed722bef65ef75dfb66ff46a.jpg" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_d19c26eb56f595ddbb8975fdec5c191b.jpg" alt="" width="">

4. 按下執行後，在對話框輸入文字，按下「✓」或鍵盤的「Enter」，可以看到小怪獸說出輸入的文字。

    <img src="https://md.webduino.io/uploads/upload_242db30b2f9ae672aeabd40343ee6215.gif" alt="" width="">

## 偵測日期時間

「偵測日期時間」積木可以偵測現在的時間，並將時間顯示在開發板或網頁上，包含的資訊有：

- 日期：年、月、日
- 時間：時、分、秒

<img src="https://md.webduino.io/uploads/upload_6869b6f0f5656ee9d00dd9c6b35d79d0.jpg" alt="" width="">

### 現在的日期 / 時間

使用時會開發板偵測現在的時間，並將資料回傳，結合其它積木就可以將時間顯示在網頁互動區或 Web:AI 上。

<img src="https://md.webduino.io/uploads/upload_972bda4409ffdd5b49e77a98c6625d47.jpg" alt="" width="">


「偵測日期時間」積木可以回傳時間 **1 次**，如果需要做出像時鐘一樣效果，就需要搭配「無限重複」積木，如下：

<img src="https://md.webduino.io/uploads/upload_148742ed92be4d06410db374b4cb8ca4.jpg" alt="" width="">

> 因為使用「偵測日期時間」積木時需要透過網路傳輸，若是在網路訊號不穩的環境下可能會讓時間顯示不穩定。

### 範例：小怪獸時鐘

1. 使用「小怪獸說話」積木搭配「偵測日期時間」積木，讓小怪獸說出日期和時間。

    <img src="https://md.webduino.io/uploads/upload_4ea034e8aef16e0b6adec1aad334f388.jpg" alt="" width="">

2. 加入「無限重複」積木及「等待」積木，設定等待 1 秒。

    <img src="https://md.webduino.io/uploads/upload_a17cb5f5bfc072b1b31a1d62eabf9d81.jpg" alt="" width="">

3. 完成積木如下，並開啟網頁互動區。

    <img src="https://md.webduino.io/uploads/upload_d3a2d75ebd1f497b8b8490d330f722d6.jpg" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_63cb78e6ed722bef65ef75dfb66ff46a.jpg" alt="" width="">

4. 按下部署，可以看到小怪獸將目前的時間說出，並隨著每秒改變。

    <img src="https://md.webduino.io/uploads/upload_fb360c76890f80462f34cc3e3484ad7f.gif" alt="" width="">
