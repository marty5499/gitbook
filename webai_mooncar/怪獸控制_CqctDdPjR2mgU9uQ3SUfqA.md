 

# 怪獸控制

Web:AI 程式積木的網頁互動區提供了 4 隻可愛的小怪獸，透過程式積木編排，就能控制每隻小怪獸的說話、展示圖片、互動等動作，甚至能進一步與實際 Web:AI 開發板互動，做出更多好玩的有趣應用。

## 小怪獸說話

「小怪獸說話」積木可以指定小怪獸，並讓小怪獸說出指定的文字。

<img src="https://md.webduino.io/uploads/upload_9a750c872d3a7f9418b4833046837ad0.png" alt="" width="">

### 範例：讓黃色小怪獸說「Hello」

1. 使用「小怪獸說話」積木，指定黃色小怪獸，輸入要讓小怪獸說的話。

    <img src="https://md.webduino.io/uploads/upload_379627966c161d71fe6af18cf34d5f07.png" alt="" width="">

2. 按下執行，可以看到黃色小怪獸說出「Hello」。

    <img src="https://md.webduino.io/uploads/upload_b2f76cc8c2ee1f66da4b97a2a25fb06a.png" alt="" width="">

## 滑鼠點擊小怪獸

「滑鼠點擊小怪獸」積木可以指定小怪獸為對象，當滑鼠點擊後，會執行後續的程式。

<img src="https://md.webduino.io/uploads/upload_f06e5a387573e0bafe904754920a52f3.png" alt="" width="">

### 範例：點擊小怪獸展示圖片

1. 使用「小怪獸展示圖片」積木，放入「LCD 顯示圖片」積木。

    <img src="https://md.webduino.io/uploads/upload_14e51682cb9d5a5f4c57de6da222b585.png" alt="" width="">


2. 指定小怪獸和要展示的圖片名稱。

    <img src="https://md.webduino.io/uploads/upload_3ec5870ad49c9b0b091b717614cff8b2.png" alt="" width="">

3. 重複 4 個，並分別設定不同小怪獸。

    - 綠色小怪獸：green
    - 紅色小怪獸：red
    - 黃色小怪獸：yellow
    - 藍色小怪獸：blue

    <img src="https://md.webduino.io/uploads/upload_aa954170268a8faae2d92fe9a394beb3.png" alt="" width="">


4. 執行後，分別點擊不同小怪獸，可以看到開發板螢幕顯示對應的小怪獸圖片。

    <img src="https://md.webduino.io/uploads/upload_97a7d977d6b9a44685aff790227a28cf.png" alt="" width="">

## 小怪獸展示圖片

「小怪獸展示圖片」積木可以讓小怪獸展示一張「網路圖片」。

<img src="https://md.webduino.io/uploads/upload_06780399df892372a632e24d069fdab5.png" alt="" width="">

### 範例：紅色小怪獸展示圖片

1. 使用「小怪獸展示圖片」積木，指定紅色小怪獸，在後方輸入網路圖片網址：https://i.imgur.com/qA6mxZU.png 。

    <img src="https://md.webduino.io/uploads/upload_b856a84c717c18104a239d0c4486e5ac.png" alt="" width="">

2. 按下執行，可以看到小怪獸將圖片展示出來。

    <img src="https://md.webduino.io/uploads/upload_9e1495cbe88f6492d19de0e4cb00aa0c.png" alt="" width="">

### 範例：小怪獸遠端拍照

1. 使用「雲端上傳圖片」積木，讓 Web:AI 拍照上傳雲端，並產生圖片網址 URL。

    <img src="https://md.webduino.io/uploads/upload_bf3758e08bfd0454198433692c077172.png" alt="" width="">

2. 配合「小怪獸展示圖片」積木，展示網址的圖片。

    <img src="https://md.webduino.io/uploads/upload_64d0aa4768c924e073cd6710078ee439.png" alt="" width="">

3. 使用「滑鼠點擊小怪獸」積木，讓綠色小怪獸作為按鈕來觸發拍照。

    <img src="https://md.webduino.io/uploads/upload_74cd15f26455820af9a4d06511782a74.png" alt="" width="">

4. 執行後，點擊綠色小怪獸即可遠端拍照，不管 Web:AI 開發板在多遠的地方都可以進行拍照並上傳到網頁互動區。

    <img src="https://md.webduino.io/uploads/upload_0a1cd1936549db40111eec5bee17c56c.png" alt="" width="">

