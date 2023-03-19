 

# 影像分類

Web:AI 影像辨識分為 **影像分類** 以及 **物件追蹤**，可以使用 Web:AI 開發板拍攝影像上傳至 Webduino 影像訓練平台進行影像訓練，將訓練完成的模型下載，再使用程式積木執行影像辨識。

本章節將會介紹「影像分類」積木的使用方式。

## 下載影像分類模型

在使用影像分類之前，需要先訓練好模型，並下載至開發板中，訓練流程歡迎參考：[三、影像訓練](./三、影像訓練_4LZCe8DqSP6T0c0KPnbJPQ.md)。

按照步驟下載後，就可以使用「影像分類」積木進行操作了。

## 設定影像分類模型

在操作影像分類前，需要先使用「設定影像分類模型」積木對模型作設定。

<img src="https://md.webduino.io/uploads/upload_7b83f05b602f41f96f9afbfeda5b9abc.jpg" alt="" width="">

- 模型：影像分類使用的模型。
- 分類：模型中的分類，使用半形逗號「,」分隔。
- 鏡頭反轉：在使用特定外殼時會有前後鏡頭功能，因此需要勾選讓鏡頭反轉，避免畫面上下顛倒。

    > 如果是使用無外殼的 Web:AI 開發板，使用預設的不勾選。
- 寬高：影像的尺寸大小。如果是使用自行訓練的模型，需要手動輸入；如果是使用 [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md) 訓練的模型，使用的尺寸則會是：
    - 寬：224
    - 高：224

在「設定影像分類模型」積木中可以選擇要使用的模型，**選擇的模型必須和下載到開發板中的板子一致**，才能順利進行辨識。

<img src="https://md.webduino.io/uploads/upload_b930030ac6820dee0c105ebbb8292520.png" alt="" width="">

選擇模型方式又會依據使用的平台及建立方式而不同，如下：

- ### 選擇模型 ( 線上版 )

    點擊「模型」，可以從下拉選單中選擇想使用的模型，選單中的模型會根據 [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md) 列出可使用的影像分類模型。

   <img src="https://md.webduino.io/uploads/upload_683d5d0a22f51326916f12ba15cf523f.png" alt="" width="">

- ### 選擇模型 ( 安裝版 )

   在「模型」中手動輸入，並將「分類」反白複製後貼上。

   > 因為分類的順序會影像到是否能正常辨識，為確保順序正確，建議直接將分類反白複製。

   <img src="https://md.webduino.io/uploads/upload_1e61f3f88871986aa8d9a891bb3977a1.jpg" alt="" width="">

- ### 選擇模型 ( 新增自訂模型 )

   如果是自行將模型燒錄進開發板，或是將模型檔案放在 SD 卡中，就需要使用「新增自訂模型」，如下方步驟：

   1. 點擊「新增自訂模型」。
   2. 輸入模型名稱，按下確定。
   3. 模型選單中出現自訂模型，後方會標示 **( 自訂 )**
   4. 在「分類」填入自訂模型的分類順序

## 開始辨識影像

使用「開始辨識影像」積木來觸發影像辨識的進行。
因為這塊積木代表觸發 1 次影像分類，如果需要重複觸發，就需要在外層放上「無限重複」積木。

<img src="https://md.webduino.io/uploads/upload_f1c7a67a2875f34be15d895bb354182c.png" alt="" width="">

## 取得辨識到的影像名稱

當開始辨識時，可以使用「取得辨識到的影像名稱」積木來顯示辨識到的分類名稱。

例如：使用模型「monster」，裡面的分類是「green,yellow,red,blue」，那麼「取得辨識到的影像名稱」積木就會是「green,yellow,red,blue」中的其中一個。

<img src="https://md.webduino.io/uploads/upload_9d457d5d878a8afca13c377475cff5b0.png" alt="" width="">

## 取得辨識到的影像信心度

當開始辨識時，可以使用「取得辨識到的信心度」積木來顯示辨識到的信心度。
信心度最高為 100、最低為 0，若信心度越高，代表偵測錯誤的可能性越低。

> 因為影像訓練辨識的結果會落在一個區間範圍內，若信心度為 90%，代表有 90% 的機率真正的結果會落在這個區間範圍內。

<img src="https://md.webduino.io/uploads/upload_47b481159799efcfda48fd36fe831bbb.png" alt="" width="">

## 範例：影像分類

1. 先從 [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md) 下載要進行影像訓練的模型，如範例是使用模型「monster」。

    > 有關如何訓練影像模型，歡迎參考：[三、影像訓練](./三、影像訓練_4LZCe8DqSP6T0c0KPnbJPQ.md)。

    <img src="https://md.webduino.io/uploads/upload_05e9f1e0bdcac076f5d9976ce9526294.jpg" alt="" width="">

2. 使用「設定影像分類模型」積木，選擇使用的模型。

    <img src="https://md.webduino.io/uploads/upload_537b21839bcd48b32795cd6e5418f789.jpg" alt="" width="">

3. 使用「無限重複」積木，放入「開始辨識影像」積木、「顯示文字」積木。

    <img src="https://md.webduino.io/uploads/upload_30a3966ae32fbd8f7c26d5cd0c503f06.jpg" alt="" width="">

4. 在「顯示文字」積木內放入要顯示的影像分類資訊，範例為顯示：**分類名稱_信心度**。

    <img src="https://md.webduino.io/uploads/upload_2239add9b2cfbb635f883fc21425971e.jpg" alt="" width="">

5. 將積木組合，按下部署即可以開始執行影像分類。

    <img src="https://md.webduino.io/uploads/upload_87abba90f956034aa9540ae021601d30.jpg" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_18ff3d4a326a6123cb54fb20940150f9.png" alt="影像辨識結果" width="">