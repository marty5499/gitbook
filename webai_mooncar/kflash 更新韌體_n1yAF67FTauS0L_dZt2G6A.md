

# kflash 更新韌體

Web:AI 開發板的韌體中使用了 2 種晶片，分別是主晶片 ( K210 ) 和 Wi-Fi 晶片 ( ESP8285 )。

Web:AI 開發板與積木平台會不斷推出新功能，使用 Web:AI 開發板之前，需要先對晶片做韌體更新，將開發板升級到最新版本，才能順利使用最全面的功能。

### Web:AI 最新版韌體：[`下載韌體`](https://webduino.s3.ap-northeast-2.amazonaws.com/webai/production-firmware/webduino/webai_latest.kfpkg)

<!-- > 韌體更新後會將 -->

## 韌體更新通知

在 Wi-Fi 設定頁面時，如果 **目前版本** 左側出現黃色小怪獸說：「前往更新韌體」，就代表目前有更新的韌體可以使用囉！

<img src="https://md.webduino.io/uploads/upload_7d8b5a393aaa85e54ded0a85bb5dc3b5.jpg" alt="" width="">

## 下載 kflash

1. 點擊 [下載 kflash](https://github.com/sipeed/kflash_gui/releases/tag/v1.6.7)，進入下載頁面。

    <img src="https://md.webduino.io/uploads/upload_c5c9f19dd053eff9a52855129358674b.png" alt="" width="">

2. 選擇符合自己電腦作業系統的檔案下載。

    <img src="https://md.webduino.io/uploads/upload_be25bd7391a751db97e4d7d830bc82cf.jpg" alt="" width="">

3. 下載之後，將檔案解壓縮，可以得到 **kflash_gui** 應用程式。未來只要有新版本韌體，只要透過 kflash_gui 就能夠直接更新了！

    <img src="https://md.webduino.io/uploads/upload_c59b565463a107beae8427aba6670257.png" alt="" width="">

## 下載 Web:AI 韌體

1. 每當要更新韌體時，只要進入本篇教學文，就可以在最上方看到最新的韌體版本。

   <img src="https://md.webduino.io/uploads/upload_c99c9f729f86dfc636d8aae0407fc582.jpg" alt="" width="">

2. 點擊連結，將韌體檔下載，可以得到 kfpkg 檔案。( 如：webai.kfpkg )

   <img src="https://md.webduino.io/uploads/upload_dcab903f77aa8f834108e0d8d26b9842.jpg" alt="" width="">

## 韌體更新步驟

1. 先將 Web:AI 開發板透過 USB 傳輸線連接上電腦。

2. 開啟 kflash_gui，介面說明如下：

   <img src="https://md.webduino.io/uploads/upload_08468177e0f20add605363d6ad11c1f0.png" alt="" width="">

3. 分別作以下設定：

    - 點擊「Open File」，選擇要燒錄的韌體檔。
    - 連接方式：選擇 USB Serial
    - 燒錄速度：選擇約 2000000 ( 數值越大代表燒錄速度越快 )

       > 如果速度過快，可能會使韌體燒錄失敗，這樣就需要先將速度調慢，再次重新燒錄。

4. 設定完成後點擊「Download」，開始進行燒錄。
   燒錄完成後會跳出視窗顯示「Dowmload success」，這時開發板會重新開機，就完成韌體更新了！

    <img src="https://md.webduino.io/uploads/upload_ce3be2497b3bbb94d08f5d14df8ffc09.png" alt="" width="">

5. 韌體更新後會將 Wi-Fi 設定清除，使用前需要先完成 Wi-Fi 設定再開始使用！
