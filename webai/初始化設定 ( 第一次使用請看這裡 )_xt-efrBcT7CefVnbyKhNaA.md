#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md)
:::info
【 更新公告 】
從現在起，我們在 [Web:AI 程式積木平台](./Web_AI 程式積木平台_.md) 提供更方便、快速的初始化設定功能，操作步驟請參考下方教學手冊。

> 關於 Wi-Fi 設定及韌體更新，歡迎參考：[Web:AI 開發板基礎設定（初次使用開發板看這裡）](./Web_AI 開發板基礎設定（初次使用開發板看這裡）_ZjV1vnESTg6uZOXC77aP8w.md)。

:::
# 初始化設定 ( 第一次使用請看這裡 )

第一次使用 Web:AI 開發板之前，需要先設定 Wi-Fi 及對晶片做韌體更新，將開發板升級到最新版本，才能順利使用最全面的功能。

#### 設定頁面：[Wi-Fi 設定頁面](./Wi-Fi 設定頁面_webai.webduino.io.md) ( 需要透過電腦的 Chrome 瀏覽器開啟 )

## 教學影片

歡迎參考下方教學影片：

<iframe src="https://www.youtube.com/embed/ZSGkZUQQXcI" allowfullscreen width="100%" style="aspect-ratio:728/410;border:none " ></iframe>

## 教學步驟：Wi-Fi 設定

當拿到 Web:AI 開發板後，只要按照步驟教學或上方影片一步步操作，就可以完成初始化設定囉！

1. 請先確認 Web:AI 開發板為預設狀態，如下圖畫面：

    <img src="https://md.webduino.io/uploads/upload_8b1389ecc47f7cfa583dcb399bfe48bd.png" alt="" width="">
    
    > 如果開發板不是預設狀態，可以參考：[操作模式：回復預設狀態](https://md.webduino.ioundefined)。

2. 首先使用電腦打開 Chrome 瀏覽器進入 [Wi-Fi 設定頁面](./Wi-Fi 設定頁面_webai.webduino.io.md)。
   ( 如果 Chrome 版本低於 89，需要先將瀏覽器更新到最新版本！)

3. 將 Web:AI 開發板透過 USB 傳輸線連接到電腦。
    ( 為避免電腦誤判，請勿插入 SD 卡 )

4. 按下「點擊開始設定」。
    <img src="https://md.webduino.io/uploads/upload_02a4681ffc6dfd1aa921e27afe17f2f5.png" alt="" width="">

5. 點擊「開始連接」。

    <img src="https://md.webduino.io/uploads/upload_792d00f7981cf19f3ffad15bf3930abf.png" alt="" width="">

6. 選擇連接 Web:AI 的 USB，點擊「連接」。

   ::: danger
   如果電腦搜尋不到 USB 裝置，請參考 [__安裝 USB 裝置驅動程式__](https://md.webduino.ioundefined) 步驟教學。
   :::
    <img src="https://md.webduino.io/uploads/upload_4892028c07de2478564d8705933f5580.png" alt="" width="">

6. 電腦連接上 Web:AI 後會出現開發板的 Device ID 和現在的韌體版本。

    <img src="https://md.webduino.io/uploads/upload_44766cf13211c94964896050340ceb25.jpg" alt="" width="500">


7. 在 Wi-Fi 連線畫面，選擇 Wi-Fi 並輸入密碼，按下「儲存連線」。

    > 如果搜尋不到 Wi-Fi，可以透過手動輸入現場的 Wi-Fi 名稱及密碼。

    <img src="https://md.webduino.io/uploads/upload_ddcfed56e5b16ca8494e8c37dc6b9bed.jpg" alt="" width="500">

8. 成功完成設定 Wi-Fi！

    <img src="https://md.webduino.io/uploads/upload_4938d84b09b19e6ff298bb8808661543.jpg" alt="" width="500">

<!-- > 如果需要進行韌體更新，再接著進行下方步驟。

## 教學步驟：更新韌體

1. 設定完 Wi-Fi 後，如果畫面有「已有新版本，點擊更新」，代表有新版本可以更新。

   點擊「更新韌體」。

    <img src="https://md.webduino.io/uploads/upload_417de60a4f044c3973890328c1ce6987.png" alt="" width="">

2. 等待韌體更新，開發板螢幕會顯示更新進度，期間內請勿斷開與 USB 線的連接。

    <img src="https://md.webduino.io/uploads/upload_73e353a9e9a08eb82c1884c0b2c8bba2.png" alt="" width="">
    <img src="https://md.webduino.io/uploads/upload_d1a8539e1deef8d0c520d7bfc5fb2b0e.png" alt="" width="">

3. 更新完成後，重新開機就可以開始使用 Web:AI 了！

    <img src="https://md.webduino.io/uploads/upload_8dbf16901021d914270ba5134b478694.png" alt="" width=""> -->

## 更新 Web:AI 韌體

在 Wi-Fi 設定頁面時，如果 **目前版本** 左側出現黃色小怪獸說：「前往更新韌體」，就代表目前有更新的韌體可以使用囉！

<img src="https://md.webduino.io/uploads/upload_87f8dab1059e57296598a2fe6f09684a.png" alt="" width="">

### 更新方式

Web:AI 韌體更新方式分為「安裝版更新」及「kflash 更新」，在使用前需要針對不同的電腦作業系統，選擇對應的更新方式。

- Windows 系統：安裝版更新、kflash 更新
- mac 及其它系統：kflash 更新

#### 歡迎前往：

- [kflash 更新韌體](./kflash 更新韌體_n1yAF67FTauS0L_dZt2G6A.md)
- [安裝版更新韌體](./安裝版更新韌體_yxI3hoLXRYuWfMyEpy0jEQ.md)

## 小提醒

- 當開發板畫面呈現與下圖 **相同** 時，才能在 Wi-Fi 設定頁面進行初始化設定。

    <img src="https://md.webduino.io/uploads/upload_9c75be672cbd440d6ee3fdb4f04b77c9.png" alt="" width="">

- 進行設定前，請先將 SD 卡移除，避免程式誤判！

- 想要再次設定 Wi-Fi 時，請先將開發板 [**回復預設狀態**](https://md.webduino.ioundefined)，當開發板顯示和上圖相同就可以進行設定。

<!-- - 若使用上述步驟卻無法更新韌體，可以參考：[安裝版更新韌體](./安裝版更新韌體_yxI3hoLXRYuWfMyEpy0jEQ.md) 來完成設定！ -->

- 如果設定頁面文字顯示為「網路：人工智能」，如下圖，代表 Chrome 瀏覽器有經過網頁自動翻譯。網頁自動翻譯會造成 Wi-Fi 設定出錯，需要將語言設定回「英文」並重新整理才能正常使用。

    <img src="https://md.webduino.io/uploads/upload_f35bd1f701c2304cac254c885f1ef660.jpg" alt="" width="500">

    <img src="https://md.webduino.io/uploads/upload_698b723317d3f9e955ac643af178d3fe.jpg" alt="" width="">
