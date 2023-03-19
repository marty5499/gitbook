

# 安裝版基礎設定

Web:AI 持續不斷推出更好用、更利於教學的功能，在新功能釋出後，需要對開發板的韌體做版本更新。另外 Web:AI 開發板也能夠因應不同的場地來設定 Wi-Fi，讓 Web:AI 在課堂中更容易達到展示、體驗，輕鬆學習 AI 與物聯網。

Web:AI 程式積木平台分為網頁版和安裝版，按照以下步驟就能在安裝版上完成基礎設定。

> 有關網頁版基礎設定，歡迎參考：[Web:AI 開發板基礎設定](./Web_AI 開發板基礎設定_ZjV1vnESTg6uZOXC77aP8w.md)。

## 下載安裝版程式積木平台

#### 下載連結：[Web:AI 安裝版](./Web_AI 安裝版_view.md)

1. 設定前先前往連結下載 Web:AI 安裝版。 
2. 下載後點擊執行，安裝完成後就可以開啟 Web:AI 安裝版了。

    <img src="https://md.webduino.io/uploads/upload_4c0c19b4782014407c134e49323fa2f4.png" alt="" width="">

## 更新韌體

Web:AI 開發板的韌體中使用了 2 種晶片，分別是主晶片 ( K210 ) 和 Wi-Fi 晶片 ( ESP8285 )。

第一次使用 Web:AI 開發板之前，需要先對晶片做韌體更新，將開發板升級到最新版本，才能順利使用最全面的功能。

### 教學影片

歡迎參考下方教學影片：

<iframe src="https://www.youtube.com/embed/vl6XY0iCCuM" allowfullscreen width="100%" style="aspect-ratio:728/410;border:none " ></iframe>

### 韌體更新步驟

1. 點擊開啟 Web:AI 安裝版。

    <img src="https://md.webduino.io/uploads/upload_4c0c19b4782014407c134e49323fa2f4.png" alt="" width="">

2. 開啟 Web:AI 安裝版，可以看到視窗最上方顯示「正在搜尋裝置...」，代表並未連接上開發板。

    <img src="https://md.webduino.io/uploads/upload_6e38bcc632aad5ef625c43833b4cd579.png" alt="" width="">

3. 透過 USB 線將 Web:AI 開發板連接上電腦，當 Web:AI 安裝版視窗顯示「已偵測到裝置」，代表成功讀取到開發板資訊。

    <img src="https://md.webduino.io/uploads/upload_cc6e863eac6b646086704d0fd37de900.png" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_01d95577c2800de0b1686ecf195a160d.png" alt="" width="">

4. 偵測到裝置後，點擊左上角「工具」，會有「更新韌體」和「更新韌體及回復原廠設定」，選擇其中一項開始進行主晶片韌體更新，視窗上方會顯示目前更新進度。

   - 更新韌體：僅更新韌體版本
   - 更新韌體及回復原廠設定：更新韌體版本並清除 Wi-Fi 設定。

    <img src="https://md.webduino.io/uploads/upload_7ba6a2e5f255c8ec78d61b4937d64f06.png" alt="" width="">

    :::danger
    更新韌體時，請勿按下 Reset 按鈕及拔除電源！若更新失敗，請再重新更新一次。
    :::

4. 韌體更新完成後，開發板會重新開機。這時 LCD 螢幕畫面如下圖，需要進一步完成 Wi-Fi 設定才能開始使用。

    <img src="https://md.webduino.io/uploads/upload_e36c621d34c0a83c433bb5ccb705de77.png" alt="" width="">

## Wi-Fi 設定

需要更改連線的 Wi-Fi 時，需要對開發板進行 Wi-Fi 設定，完成後就能夠讓開發板連上網路。安裝版使用「 QR Code 設定」，不需要透過 USB 連接電腦也可以設定 Wi-Fi。

若是使用網頁版程式平台，則是透過 USB 設定 Wi-Fi。

> 關於使用 USB 設定 Wi-Fi，歡迎參考：[Web:AI 基礎設定](./Web_AI 開發板基礎設定_ZjV1vnESTg6uZOXC77aP8w.md)。

### 步驟

1. 在 Web:AI 程式積木中，點擊「WiFi 設定」按鈕，

    <img src="https://md.webduino.io/uploads/upload_968fc0eceabcccc185b7bc2a546b1d71.jpg" alt="" width="">

2. 跳出「WiFi 設定」視窗，輸入 SSID 和密碼後，點擊「設定」，進入 QRcode 頁面。

    - SSID：欲連線的 Wi-Fi 名稱
    - 密碼：Wi-Fi 密碼

   <img src="https://md.webduino.io/uploads/upload_6f7e320080816647d62cb09c622b046b.png" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_9bbf3a19c931f8b93d79f517ac190dd9.png" alt="" width="">

3. 按下開發板上的 **Reset 按鈕**，在 5 秒內按下 **R 按鈕**，進入 QR Code 掃描模式。

   <img src="https://md.webduino.io/uploads/upload_e8089a96c7e5bad6ab60d9253aa5ba8a.png" alt="" width="">

4. 使用開發板鏡頭對準 QR Code 掃描，進入 Wi-Fi 設定流程。

5. 設定完成後開發板會重新啟動，畫面會顯示：
    - Device ID
    - 韌體版本
    - Wi-Fi 名稱及狀態

    當螢幕顯示綠色「Wi-Fi Connected」，就代表開發板成功連上網路了；如果出現紅色「Wi-Fi Failed」代表並未連上網路，請確認網路訊號及密碼是否正確。

    <img src="https://md.webduino.io/uploads/upload_73acc92e869132db14f17349bdb706df.png" alt="" width="">

   > Wi-Fi 狀態後方括號的數字代表網路訊號強度，數字越大代表訊號越強，建議 -50dBm 以上使用較順暢。
   > ( 如：-40dBm 訊號優於 -70dBm )

## 執行程式

安裝版程式積木平台使用 USB 離線部署程式，因此即使開發板未連上網路也能夠燒錄程式。

1. 將 Web:AI 開發板透過 USB 傳輸線連接上電腦。

    <img src="https://md.webduino.io/uploads/upload_969b2029125090a94b21739c33b9c065.png" alt="" width="">

2. 確認積木平台顯示「已偵測到裝置」。

    <img src="https://md.webduino.io/uploads/upload_f5c3285f9aacefd1398bb349cc480843.png" alt="" width="">

3. 點擊右上角「範例」，挑選一個範例，如「左顧右盼」。

    <img src="https://md.webduino.io/uploads/upload_0335bdf84099424830f587169f6d9be8.jpg" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_35f1b77a6c3e34063f2f2804a16d22dd.png" alt="" width="">

4. 開啟範例後，按下「執行」。

    <img src="https://md.webduino.io/uploads/upload_452d3d40bfc988bfb56aa601eef14408.jpg" alt="" width="">

5. 等待程式部署後，就可以看到 Web:AI 成功執行程式了！

    <img src="https://md.webduino.io/uploads/upload_10eaae1a28675183e916965ac919fa61.gif" alt="" width="">

