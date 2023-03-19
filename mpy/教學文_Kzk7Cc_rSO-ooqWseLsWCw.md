# WebEye Pro 使用手冊

**讓 WebEye Pro 為您捕捉精彩的每一刻！**

<img src="https://md.webduino.io/uploads/upload_71452992bd71a48b3dd9b5bd5335d405.png" alt="" width="49%"><img src="https://md.webduino.io/uploads/upload_532a995451e2ad76aabd5fb245c012f1.jpg" alt="" width="50%">



不論食農教育還是生態觀察，想要記錄生物生長的點滴，光是文字敘述絕對是不夠的，出色的照片或影片，能幫助我們更精準的捕捉生命成長的感動。然而專業的攝影器材既昂貴、又有一定的技術門檻，加上需要到現場按下快門才能拍攝，一般人想要透過影像完整記錄生物的生長過程並不容易。

Webduino 推出的 WebEye Pro ，透過物聯網（ IoT ）技術，只要設備上線，**不論您在哪裡，都能透過可以上網的手機、平板、電腦查看現場狀況，並且拍照上傳 Google 雲端硬碟。** 更棒的是，WebEye Pro 提供**定時快門**功能，只要將拍好的照片匯入影片剪輯軟體，就能輕鬆做出吸睛的生態縮時影片！

手上有 WebEye Pro 了嗎？現在就讓我們跟著下面的步驟設定吧！

---

**【目錄】**
[TOC]

## 一、規格
內容物：WebEye Pro、USB 充電頭、固定用螺絲（ ×3 ）、說明小卡

<img src="https://md.webduino.io/uploads/upload_e70d35227965d0081201aa8b39a1e773.jpg" alt="" width="">


## 二、讓 WebEye Pro 連上 Wi-Fi
使用 WebEye Pro 之前，最重要的就是進行初始化設定，初始化設定的目的在於讓 WebEye Pro 可以自動連上 Wi-Fi。
### 1. 接上電源
第一步就是接上電源，此時 WebEye Pro 會閃紅燈。
<img src="https://md.webduino.io/uploads/upload_8c601f4e1ea2df9b185fc6658a6cc7c4.gif" alt="" width="100%">

### 2. 將電腦或行動裝置連上 WebEye Pro 熱點
接著，在具備 Wi-Fi 功能的電腦或行動裝置的 Wi-Fi 搜尋清單裡，可以看到您的 WebEye Pro 無線網路名稱（ 請查看外殼或說明小卡上的 SSID，出廠時預設為 wdXXX ）。

點選該無線網路後，輸入預設密碼 ```12345678```，進行連線。

> 此時若出現「此網路無連線能力」的提示是正常的。

<img src="https://md.webduino.io/uploads/upload_bc71f0569aaa6884dc9ca45c167cf610.png" alt="" width="100%">

### 3. 設定 Wi-Fi 帳號密碼
確認連線成功後，打開瀏覽器 ( 建議使用 Chrome )，網址列輸入：```192.168.4.1 ```，將前往 WebEye Pro 的 Wi-Fi 設定畫面。

在「 Wi-Fi 」分頁中的「 Wi-Fi No.1 」填入您的 Wi-Fi 基地台名稱（SSID）和密碼（PWD），表示 WebEye Pro 要連接哪個 Wi-Fi 基地台。
> 目前每台 WebEye Pro 限綁定一組 Wi-Fi。 

<img src="https://md.webduino.io/uploads/upload_e858baa6eabf89cc52a5e25402b481f6.jpg" alt="" width="100%">


設定完成後畫面往下滑，按下「SUBMIT」儲存。

<img src="https://md.webduino.io/uploads/upload_008d87a55d51c7b234d015330c4b0f6d.png" alt="" width="100%">

當畫面出現「Save OK, Restart...」的文字表示儲存成功，此時 WebEye Pro 會開始嘗試和您設定的 Wi-Fi 基地台連線。當紅燈熄滅，表示已經成功連結上環境內的 Wi-Fi 基地台。
> 若紅燈持續閃爍，代表沒有成功連上 Wi-Fi，需重複步驟「3. 設定 Wi-Fi 帳號密碼」。

確認 WebEye Pro 上線後，您就可以將電腦或行動裝置連回平常使用的網路環境。

<img src="https://md.webduino.io/uploads/upload_6de2feb7a60acff9cc4d4612be2d0783.png" alt="" width="100%">

## 三、使用「WebEye Pro 遙控器」遠端記錄影像
###   1. 建立 Google 雲端資料夾
   登入您的 Google 帳號，在 Google 雲端硬碟建立一個資料夾。接著將連結分享權限設定為「任何知道這個連結的網際網路使用者都能編輯」，然後複製連結。
   
<img src="https://md.webduino.io/uploads/upload_7b78a453410d53c36d38dbc22850f2cc.png" alt="" width="100%">

### 2. 設定「WebEye Pro 遙控器」
   使用手機掃描 WebEye Pro 機身的 QR Code，進入您的「WebEye Pro 遙控器」。（ 建議使用 Chrome 瀏覽器 ）
>    或是在瀏覽器輸入網址：https://webeye-pro.webduino.io/?deviceId=deviceId ( 等號後面填入 DevID。 )
>    例如：若您的 DevID 為 cfh34v，則輸入網址：https://webeye-pro.webduino.io/?deviceId=cfh34v
    
<img src="https://md.webduino.io/uploads/upload_bc896fe79ec47b918028cd8991a564e5.jpg" alt="" width="100%">

>    每個 WebEye Pro 上的 QR Code 都是獨一無二的，所以每個 WebEye Pro 都有專屬的遙控器喔！

您可以從遙控器上方得知 WebEye Pro 是否上線。

<img src="https://md.webduino.io/uploads/upload_82b7e5584f1209d0e5d5e78bd0c60016.png" alt="" width="100%">

<img src="https://md.webduino.io/uploads/upload_3f1231893546acf399ec7c7cb45e14b2.png" alt="" width="100%">



「WebEye Pro 遙控器」共有三個按鈕，從左到右依序為：

設定定時拍照、拍攝一張照片、設定雲端資料夾。

<img src="https://md.webduino.io/uploads/upload_5a1672c8d7c34c6db173e4e1efe5eb85.png" alt="" width="100%">


點擊「設定雲端資料夾」按鈕，將剛才複製的資料夾連結在輸入框貼上，然後點擊「送出」儲存設定。

<img src="https://md.webduino.io/uploads/upload_85b9af6d391a8312c032d08c8f79b4f3.png" alt="" width="100%">

完成設定後，只要 WebEye Pro 是上線狀態，點擊「拍攝一張照片」，就會顯示現場即時影像，同時自動上傳至您的雲端資料夾。



**WebEye Pro 也可以設定「定時拍照」，每隔一段時間自動拍攝照片。** 點擊「設定定時拍照」，將開關拉至「開」，選擇每次拍照間隔的時間，點擊「送出」，WebEye Pro 就會定時拍照並上傳雲端資料夾。
>   例如：選擇「 5 分鐘」代表每 5 分鐘自動拍照一次。）

<img src="https://md.webduino.io/uploads/upload_dac00618761f81efeeb95da95f19a3bd.png" alt="" width="100%">


## 四、進階功能：使用 colab 製作縮時影片
> 以下步驟建議使用電腦執行。
1. 登入您的 Google 帳號。（需和儲存照片的雲端資料夾同一個帳號）
2. 👉  [前往 colab 製作縮時影片](https://colab.research.google.com/drive/1EtJ1B-86VOTZjdu2jWpsXMQeCZGFZrgy?usp=sharing)
3. 在「選擇資料夾目錄」輸入您儲存照片的雲端資料夾名稱。（ 下圖紅框處 ）
> 資料夾名稱務必輸入正確，否成程式會執行錯誤。( 若資料夾不是存在雲端硬碟的根目錄，則名稱要輸入資料夾路徑。例如：A資料夾/B資料夾/WebEyePro )

<img src="https://md.webduino.io/uploads/upload_6e7f649560bb999a52a593b7e3fd74d8.png" alt="" width="100%">

  
4. 在工具列選擇「 Runtime 」>「 Run all 」。<img src="https://md.webduino.io/uploads/upload_023d209c53a28c5049b6e37678d08375.png" alt="" width="100%">

5. 等待程式執行幾秒後，會跳出提示，選擇「 Run anyway 」。 <img src="https://md.webduino.io/uploads/upload_a8467264a20ffc224711f6c98f87464d.png" alt="" width="100%">

6. 接著 colab 會詢問是否連接至您的 Google 雲端硬碟，選擇「 Connect to Google Drive 」。<img src="https://md.webduino.io/uploads/upload_66546c410be2907256d49bb45e57237d.png" alt="" width="100%">

8. 選擇要連接的 Google 帳號。<img src="https://md.webduino.io/uploads/upload_6192945aee489dc2cdd745da08d65577.jpg" alt="" width="100%">
9. 選擇「允許」同意授權。<img src="https://md.webduino.io/uploads/upload_c2a8cf1c5a29ed846a9b1d9037b4edb9.png" alt="" width="100%">
10. 待程式執行完成後，會自動下載產生的縮時影片到您的電腦。 <img src="https://md.webduino.io/uploads/upload_ddc2365b5bdc7379a228ad9c1d8970aa.png" alt="" width="100%"> 同時，也會在您的 Google 雲端硬碟備份這支影片。<img src="https://md.webduino.io/uploads/upload_be4aaaa15a6b3d476718d5125f1e8d55.jpg" alt="" width="100%">









## 五、常見問題
:::spoiler 1. **為什麼我的電腦或行動裝置無法連上 WebEye Pro 的熱點？**

與 WebEye Pro 進行連線時，請確認 WebEye Pro 在您的附近，且中間無牆壁或大型電器阻隔，以免干擾訊號。

若您使用行動裝置與 WebEye Pro 進行連線，請先關閉行動裝置的行動數據再進行設定。

:::
---
:::spoiler 2. **為什麼 WebEye Pro 無法連上環境內的 Wi-Fi？**

WebEye Pro 一直無法連上環境的 Wi-Fi ，其中一個原因是 Wi-Fi 沒有設定成功。請先確認您在步驟「 3. 設定 Wi-Fi 帳號密碼 」設定的 Wi-Fi 基地台名稱（ SSID ）和密碼（ PWD ）輸入正確。 

此外，請確認 Wi-Fi 基地台訊號源在 WebEye Pro 附近，且訊號強度足夠。

若還是無法上線，可嘗試重新插拔 WebEye Pro 電源，或是關閉遙控器網頁後，重新掃描 QR Code 再次進入遙控器畫面。
:::
---
:::spoiler 3. **如何變更 WebEye Pro 連接的 Wi-Fi 基地台？**
重複本文步驟「 二、讓 WebEye Pro 連上 Wi-Fi 」，在設定 Wi-Fi 基地台時輸入另外一組 Wi-Fi 基地台名稱（ SSID ）和密碼（ PWD ），就可以囉！
:::
---
:::spoiler 4. **同一個 WebEye Pro 的遙控器可以分享給多個人使用嗎？**
可以的！只要將遙控器的連結分享給您的親友，他們也可以透過他們的電腦或行動裝置遙控拍照。
> 小叮嚀：遙控器設定會以最後一個人的設定內容為準。
:::
---
:::spoiler 5. **WebEye Pro 需要和電腦連一樣的 Wi-Fi 嗎？**
不需要。WebEye Pro 使用物聯網技術控制，只要 WebEye Pro 上線，電腦或行動裝置就能從遠端控制，不需要在同一個網路環境內。
:::
---
:::spoiler 6. **WebEye Pro 有拍攝照片數量的上限嗎？**
沒有。WebEye Pro 拍攝的照片儲存在您的 Google 雲端硬碟，只要您的雲端硬碟儲存空間足夠，WebEye Pro 就能持續拍照上傳。而且您隨時都能到雲端硬碟查看和下載照片，再也不需要為了拔攝影機裡的記憶卡來回奔波。
:::







---
## 聯絡我們
如果對於 Webduino 產品有興趣，歡迎透過下列方式購買：

> 個人線上購買：https://store.webduino.io/ ( 支援信用卡、超商取貨付款 )
> 企業＆學校採購：來信 service@webduino.io 或來電 07-3388511。

如果對於這篇教學有任何問題或建議，歡迎透過下列方式聯繫我們：

> Email： service@webduino.io 
> Facebook 粉絲團：https://www.facebook.com/webduino/
> Facebook 技術討論社團：https://www.facebook.com/groups/webduino/
> 
---
