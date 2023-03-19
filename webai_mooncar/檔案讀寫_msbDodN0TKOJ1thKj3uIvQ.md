 

# 檔案讀寫

Web:AI 檔案讀寫功能能夠將鏡頭拍攝的圖片存入，並透過 LCD 螢幕顯示的功能將儲存的圖片展示出來。透過檔案讀寫功能，可以讓 Web:AI 開發板實現照相機、自拍等影像應用。

> 更多相關應用，可以參考：[LCD 顯示圖片](https://md.webduino.ioundefined)。

## 寫入檔案

「寫入檔案」積木可以將鏡頭捕捉到的影像儲存在開發板記憶體中，再配合其它積木展示。

<img src="https://md.webduino.io/uploads/upload_0467957e1aab1208df0cc8fb9732b98a.png" alt="" width="">

## 圖片 ( 檔案 )

「圖片 ( 檔案 )」積木要使用的圖片，能夠根據圖檔的名稱加以讀取並使用。

<img src="https://md.webduino.io/uploads/upload_9844d06a3efc96392cd124fc7b783432.png" alt="" width="">

### 應用範例：自拍照相

1. 先設定拍照狀態，使用「無限重複」積木讓開發板保持在拍照狀態。

    <img src="https://md.webduino.io/uploads/upload_71ff8223a0f878a61c8e80c7fb05d899.png" alt="" width="">

2. 使用「變數 show」來表示相機的狀態，開發板一開始會保持在拍照狀態。
 
   <img src="https://md.webduino.io/uploads/upload_5c5a38e6240f641e002335da3812879c.png" alt="" width="">

    - 真：展示拍攝的照片
    - 假：拍照狀態

3. 設定當 L 按鈕按下，會拍攝照片，並同時顯示「儲存中...」和「完成」。

   <img src="https://md.webduino.io/uploads/upload_1f2b11380cf2372c9ca3672bd50efa3f.png" alt="" width="">

4. 設定當 R 按鈕按下，會顯示拍攝的照片。

    <img src="https://md.webduino.io/uploads/upload_d7494a77b30b1496ed4d98822662f13e.png" alt="" width="">

5. 設定當 R 按鈕放開，「變數 show」為**假**，回到拍照狀態。

    <img src="https://md.webduino.io/uploads/upload_90628981c80e3f7c9dde48fdf506bfe6.png" alt="" width="">

6. 完成後開始執行，按下開發板 L 按鈕拍照，按下 R 按鈕展示。

    <img src="https://md.webduino.io/uploads/upload_4926d849dc1ccd16171bfbe981df306f.png" alt="" width="">

<img src="https://md.webduino.io/uploads/upload_137463eb3594996be60e6b4514feba5e.gif" alt="" width="">

## 圖片雲端上傳

「圖片雲端上傳」積木能夠將開發板中的圖檔上傳至雲端空間「Webduino 小口袋」。

如下方積木代表：拍攝一張照片，命名為「pic」後上傳雲端，將雲端網址設定為變數「URL」。

<img src="https://md.webduino.io/uploads/upload_2dc7c9b82c89bc694a7cdec9b113d12d.png" alt="" width="">

### 應用範例：拍照上傳小口袋

#### ➤ 前往 [`範例連結`](https://ai-blockly.webduino.io?hashid=vYrloQR8Yr)

1. 使用「圖片雲端上傳」積木搭配「按鈕」積木，按下 L 按鈕能夠拍一張照片上傳到 Webduino 小口袋。

    <img src="https://md.webduino.io/uploads/upload_6a927334db7587ae7314610481c8b2e1.png" alt="" width="">

2. 加入小怪獸積木，讓綠色小怪獸說出雲端網址、紅色小怪獸展示圖片。

    <img src="https://md.webduino.io/uploads/upload_35f512c5308ac51d39cf4b2c2d7f83e9.png" alt="" width="">

3. 執行後，按下 L 按鈕，可以拍照上傳，並用小怪獸顯示出來。

    <img src="https://md.webduino.io/uploads/upload_0aaa0536a2ce24b5061e3375354bcc55.png" alt="" width="">

## 圖片雲端下載

「圖片雲端下載」積木可以將「Webduino 小口袋」的圖片下載到開發板中，能夠搭配「LCD 顯示圖片」積木將圖片顯示出來。

<img src="https://md.webduino.io/uploads/upload_b42f74b9145c7b64c4cd421a3ce9a194.png" alt="" width="">

<img src="https://md.webduino.io/uploads/upload_91484cbd0371f10fd54c27ac8738c951.png" alt="" width="">

### 應用範例：顯示雲端圖片

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 先使用「圖片雲端上傳」積木將圖片命名，上傳至 Webduino 小口袋。
2. 使用「圖片雲端下載積木」，設定雲端圖片的檔名，如上傳雲端的圖片名稱為「apple」，則將檔名設定為「apple」。

    <img src="https://md.webduino.io/uploads/upload_7638a1d8d5e3a1180ed150fc99c477d8.png" alt="" width="">

3. 搭配「LCD 顯示圖片」積木，可以讓開發板顯示下載的雲端圖片。

    <img src="https://md.webduino.io/uploads/upload_d10cdbdd187e5abc45c716ae3899de6c.png" alt="" width="">

## 下載圖片

「下載圖片」積木可以設定網路圖片的網址，並將圖片下載到開發板中。

<img src="https://md.webduino.io/uploads/upload_4468a4040153893a6d02fd13287f6f6f.png" alt="" width="">

## 應用範例：下載網路圖片

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 在瀏覽器中搜尋圖片，如下圖搜尋「webai」。

    <img src="https://md.webduino.io/uploads/upload_32ec68d2973fc6a5722fd8ced155de7e.png" alt="" width="">

2. 找到想下載的圖片，按下右鍵，點擊「複製圖片位址」。

    <img src="https://md.webduino.io/uploads/upload_5c5984a4171e9c14e2873d0beec96dd6.png" alt="" width="400">

3. 將複製的圖片位址貼在積木的網址中，並設定圖片檔名。

    <img src="https://md.webduino.io/uploads/upload_9ff99219611b1ed8583771b6c7f8982c.png" alt="" width="">

4. 使用「LCD 顯示圖片」積木將圖片顯示出來。

    <img src="https://md.webduino.io/uploads/upload_3d94b3fb592310fde1e4740554fbb21e.png" alt="" width="">
    
    <img src="https://md.webduino.io/uploads/upload_1bc8ead267553d132ec6c3bf0b6db528.png" alt="" width="">
