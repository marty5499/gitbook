

# 語音辨識

Web:AI 能夠將收錄到的聲音轉換成訊號，經過處理後儲存成聲音模型，當偵測到聲音時，會開始和開發板儲存的聲音模型比對音色、頻率，進而得到辨識結果。

## 錄製語音

「錄製語音」積木能夠透過開發板上的麥克風接收聲音訊號，並將訊號轉換成聲音模型儲存，開發板中最多可以同時儲存 10 個模型並做辨識。

- 錄音的時間約 1.5 秒
- 錄製完的聲音模型會一直存放在開發板中，除非經過韌體更新或是錄製相同編號模型覆蓋。

<img src="https://md.webduino.io/uploads/upload_35bfe0c86f4fe079f23d9c4ed1cf72e1.png" alt="" width="">

> 使用「錄製語音」積木建立聲音模型並不會覆蓋 **教學範例卡：語音互動** 中的聲音模型，可以放心使用！
> 
> 歡迎參考：[教學範例卡使用教學：語音互動](./教學範例卡使用教學：語音互動_md.webduino.ioundefined.md)。

## 語音辨識

當開發板的麥克風偵測到聲音時，如果符合聲音模型，就會自動執行「語音辨識」積木中的內容。

<img src="https://md.webduino.io/uploads/upload_84a175743d91231364e358a130dc5fe9.jpg" alt="" width="">

「語音辨識」積木的號碼和名稱會和「錄製語音」積木互相對應。

<img src="https://md.webduino.io/uploads/upload_e61839237fec9517099e535434064a9f.png" alt="" width="">

## 語音辨識門檻

因為每個人的音色、頻率都不同，所以針對不同應用需要調整辨識門檻才能達到合適的效果。
而「語音辨識門檻」是語音辨識的精準度，門檻越高代表聲音越像才會辨識成功。

> 「語音辨識門檻」積木需要放在「語音辨識」積木之前！

<img src="https://md.webduino.io/uploads/upload_d5a69cbf6a0cff9e9bf5c5c66cb077a5.jpg" alt="" width="">

## 範例：聲控圖案

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

### 錄音

1. 結合「畫文字」積木和「錄製語音」積木，錄音時顯示「請說 XX」；錄音完成時顯示「錄音 XX 完成」。

    <img src="https://md.webduino.io/uploads/upload_874d1de7d96a0bce1df0c6b344ea4c65.png" alt="" width="">

2. 做出另一組相同的積木，如下圖：

    <img src="https://md.webduino.io/uploads/upload_278aa7293c58b306ce8359fda8feac76.png" alt="" width="">

3. 將 1. 和 2. 的兩組積木組合，並用「等待」積木和「清除 LCD 畫面積木」隔開，再放入「函式」積木中，將函式命名為「錄音」。

    <img src="https://md.webduino.io/uploads/upload_277fede13002d8fcfe8e205a61494216.jpg" alt="" width="">

4. 將函式「錄音」放入「開發板」積木中，在下方再放入其它積木，如下圖即完成錄音程式。

   <img src="https://md.webduino.io/uploads/upload_2074f0bf5244ad2996764e6ee4f5edd7.jpg" alt="" width="">

### 辨識

1. 首先放入「語音辨識門檻」積木，可以根據辨識的狀況改變門檻高低。

   <img src="https://md.webduino.io/uploads/upload_8b9cd5eb6eb2a855a7e8560c7b70c765.jpg" alt="" width="">

2. 使用「語音辨識」積木，當聽到錄製的單詞時，會做出後續的程式。

    <img src="https://md.webduino.io/uploads/upload_608e2765058f13e124cedfcbe1521f1c.jpg" alt="" width="">

3. 複製 2. 的積木，並做出另一組積木。

    <img src="https://md.webduino.io/uploads/upload_4b8c00e2106272522dfaaf87b8811d4f.jpg" alt="" width="">

4. 將積木組合，按下執行即可開始語音辨識。

<img src="https://md.webduino.io/uploads/upload_6a2118831450e68215943573fe374108.jpg" alt="" width="">

<img src="https://md.webduino.io/uploads/upload_c072b055bcc2a28e37dfff15ff464567.gif" alt="" width="">


<!-- ## 範例：辨識 4 色語音

### 錄音

1. 結合「畫文字」積木和「錄製語音」積木，並用「函式」積木將積木組合。

    <img src="https://md.webduino.io/uploads/upload_7f575d4dbc80a72fad033bfd904d5938.jpg" alt="" width="">

2. 複製出 3 組同樣的積木，更改成「藍色」、「綠色」、「黃色」，做出如下圖。

> 記得更改：
> - 函式名稱
> - 畫文字
> - 語音號碼
> - 語音名稱

<img src="https://md.webduino.io/uploads/upload_4304cc17c12b575ab5e505487ce254c2.jpg" alt="" width="">

3. 將「函式」積木放入「開發板」積木中，並用「清除 LCD 畫面」積木區隔，避免文字被覆蓋。

    <img src="https://md.webduino.io/uploads/upload_87fc803ae4e31489b44b56ea4525dee3.jpg" alt="" width="">

### 辨識 -->
