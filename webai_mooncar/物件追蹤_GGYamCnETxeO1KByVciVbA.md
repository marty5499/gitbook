 

# 物件追蹤

Web:AI 影像辨識分為 **影像分類** 以及 **物件追蹤**，可以使用 Web:AI 開發板拍攝影像上傳至 Webduino 影像訓練平台進行影像訓練，將訓練完成的模型下載，再使用程式積木執行影像辨識。

本章節將會介紹「物件追蹤」積木的使用方式。

## 下載物件追蹤模型

在使用物件追蹤前，需要先訓練好模型，並下載至開發板中，訓練流程歡迎參考：[三、影像訓練](./三、影像訓練_4LZCe8DqSP6T0c0KPnbJPQ.md)。按照步驟下載後，就可以使用「物件追蹤」積木進行操作了。

另外，也可以直接使用已經訓練完成的「小怪獸模型」，內建在開發板中不需要重新訓練及下載模型。

## 設定物件追蹤模型

在操作物件追蹤前，需要先使用「設定物件追蹤模型」積木對模型作設定。

<img src="https://md.webduino.io/uploads/upload_97f798f5724f2a66ecc226e130018997.jpg" alt="" width="">

- 模型：物件追蹤使用的模型。
- 分類：模型中的分類，使用半形逗號「,」分隔。
- 辨識門檻：物件追蹤的精準度，門檻越高代表偵測越像才會辨識成功，預設為 0.5。
- 鏡頭反轉：在使用特定外殼時會有前後鏡頭功能，因此需要勾選讓鏡頭反轉，避免畫面上下顛倒。

    > 如果是使用無外殼的 Web:AI 開發板，使用預設的不勾選。
- 寬高：影像的尺寸大小。

    1. 內建「小怪獸模型」，使用的尺寸：
        - 寬：320
        - 高：224
    2. [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md) 訓練的模型，使用的尺寸：
        - 寬：224
        - 高：224
    3. 使用自行訓練的模型，需要手動輸入。

在「設定物件追蹤模型」積木中可以選擇要使用的模型，選擇的模型必須和下載到開發板中的板子一致，才能順利進行辨識。

<img src="https://md.webduino.io/uploads/upload_21d3cc0c20de32a7f4c57215bc3d776e.png" alt="" width="">

選擇模型方式又會依據使用的平台及建立方式而不同，如下：

- ### 選擇模型 ( 線上版 )

    點擊「模型」，可以從下拉選單中選擇想使用的模型，選單中的模型會根據 [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md) 列出可使用的影像分類模型，也可以選擇開發板內建的 **小怪獸模型 ( 預設模型 )**。

    <img src="https://md.webduino.io/uploads/upload_dbf7e9a32bb8838a990fa3dd489b3592.jpg" alt="" width="">

- ### 選擇模型 ( 安裝版 )

   在「模型」中手動輸入，並將「分類」反白複製後貼上。

   > 因為分類的順序會影像到是否能正常辨識，為確保順序正確，建議直接將分類反白複製。

   <img src="https://md.webduino.io/uploads/upload_ae8f3f322f44afec3e12d1f4c56b5ccc.jpg" alt="" width="">


    -  使用小怪獸模型 ( 預設模型 )
        1. 使用「設定模型積木」。在「模型」中手動輸入模型名稱 monster
        2. 在「分類」中手動輸入分類 green,yellow,red,blue
        2. 辨識門檻：0.1 ( 建議 )
        3. 鏡頭反轉：在使用特定外殼時會有前後鏡頭功能，因此需要勾選讓鏡頭反轉，避免畫面上下顛倒。

        > 如果是使用無外殼的 Web:AI 開發板，使用預設的不勾選。
        5. 寬高：影像的尺寸大小。寬：320；高：224。

        填寫範例：
    
        <img src="https://md.webduino.io/uploads/upload_6ee323b7c20f5f63ee1c17a88b87d5d0.png" alt="" width="">

    -  使用 Webduino 影像訓練平台訓練的模型
        1. 使用「自訂模型積木」。
        2. 填寫分類：在影像訓練平台選擇欲使用的模型，將「分類」反白複製後貼上。

        > 因為分類的順序會影像到是否能正常辨識，為確保順序正確，建議直接將分類反白複製。

       <img src="https://md.webduino.io/uploads/upload_ae8f3f322f44afec3e12d1f4c56b5ccc.jpg" alt="" width="">
       
       3. 填寫 anchor 資訊：在影像訓練平台點擊欲使用的模型，選擇「模型資訊」>「複製」。將複製的內容，填入積木的「anchor」欄位。
    
            <img src="https://md.webduino.io/uploads/upload_fadf2d8f933321a03585abc2a596fdc1.gif" alt="" width="">
    
        3. 辨識門檻：0.5 ( 建議 )
        4. 鏡頭反轉：在使用特定外殼時會有前後鏡頭功能，因此需要勾選讓鏡頭反轉，避免畫面上下顛倒。

        > 如果是使用無外殼的 Web:AI 開發板，使用預設的不勾選。
        6. 寬高：影像的尺寸大小。寬：224；高：224。
    
        填寫範例：

        <img src="https://md.webduino.io/uploads/upload_bb721bf21d8688f16b00f2c0e35b6953.png" alt="" width="">



- ### 選擇模型 ( 新增自訂模型 )

   如果是自行將模型燒錄進開發板，或是將模型檔案放在 SD 卡中，就需要使用「新增自訂模型」，如下方步驟：

   1. 點擊「新增自訂模型」。
   2. 輸入模型名稱，按下確定。
   3. 模型選單中出現自訂模型，後方會標示 **( 自訂 )**
   4. 在「分類」填入自訂模型的分類順序

## 開始偵測物件

使用「開始偵測物件」積木來觸發影像辨識的進行。
因為這塊積木代表觸發 1 次物件追蹤，如果需要重複觸發，就需要在外層放上「無限重複」積木。

<img src="https://md.webduino.io/uploads/upload_27aa790cf95ff9db5294d9df1b840e8b.png" alt="" width="">

## 取得所有物件

當開始辨識時，使用「取得所有物件」積木來取得偵測到的物件。
積木裡面需要填入分類的名稱。

<img src="https://md.webduino.io/uploads/upload_41c2c3450b6a2e6766038edb6a535789.png" alt="" width="">

使用時可以搭配「變數」積木，讓後續程式更方便撰寫，如下方程式為：將偵測到的「分類 green」用變數命名為「objGroup」。

<img src="https://md.webduino.io/uploads/upload_c64000adb0b2347ae0d3d749d4e1b51e.png" alt="" width="">


## 物件資訊

當開始辨識時，可以使用「物件資訊」積木來顯示辨識到的資訊，包含：x 座標、y 座標、寬、高、信心度。( 信心度最高為 1、最低為 0，若信心度越高，代表偵測錯誤的可能性越低。)

> 因為影像訓練辨識的結果會落在一個區間範圍內，若信心度為 90%，代表有 90% 的機率真正的結果會落在這個區間範圍內。

<img src="https://md.webduino.io/uploads/upload_88123d415bc525a5ca7d6d5de7660644.png" alt="" width="">


## 範例：物件追蹤內建小怪獸模型

#### ➤ 前往 [`範例連結`](./`範例連結`_.md)

1. 先選擇要使用的模型，如範例是使用開發板內建的小怪獸模型「monster ( 預設模型 )」。

    > 如果不使用內建模型，就需要先從 [Webduino 影像訓練平台](./Webduino 影像訓練平台_.md) 下載。
    > 有關如何訓練影像模型，歡迎參考：[三、影像訓練](./三、影像訓練_4LZCe8DqSP6T0c0KPnbJPQ.md)。

2. 使用「設定物件追蹤模型」積木，選擇使用的模型。

    <img src="https://md.webduino.io/uploads/upload_ff8eb029745adb0bb1d5102eb1609e8f.png" alt="" width="">


3. 使用「無限重複」積木，放入「開始偵測物件」積木，代表不斷觸發物件追蹤。

    <img src="https://md.webduino.io/uploads/upload_5c554f74a0d25541309ca409ed40c63d.png" alt="" width="">

4. 使用「變數」積木，將偵測到的所有「分類 green」命名為「greenGroup」。

    <img src="https://md.webduino.io/uploads/upload_a047c40154e91ae194d63539628e697b.png" alt="" width="">

5. 使用「邏輯」積木及「陣列長度」積木，當偵測到的「green」數量 ≥ 1，會執行後方程式。
 
    > 當鏡頭偵測到的綠色小怪獸數量 ≥ 1，就會執行後方程式。

    <img src="https://md.webduino.io/uploads/upload_be9fd458ac6eb9dedc9118cc4b80a22c.png" alt="" width="">

6. 在執行後方放入「變數」積木，將「陣列 greenGroup」的第一項命名為「green」。

    > 因為物件追蹤可以同時追蹤多個物件，但是只能同時顯示單一物件的資訊，所以設定為「陣列 greenGroup」中的第一個。

    <img src="https://md.webduino.io/uploads/upload_6943d7d1fc6dde1d9dbdabe0065dc54f.png" alt="" width="">

7. 在後方放入「顯示文字」積木，顯示「變數 green」的資訊。

    > 當偵測到綠色小怪獸時，顯示「Green Monster!( x 座標,y 座標 )」

    <img src="https://md.webduino.io/uploads/upload_2e1df523b6b44510fa94d7d4e847c313.png" alt="" width="">

8. 將積木組合後，按下部署即可追蹤小怪獸，並顯示綠色小怪獸的座標位置。

    <img src="https://md.webduino.io/uploads/upload_b0a73531d00d5e1d4ce5f622ee83929e.png" alt="" width="">

9. 另外再重複步驟 4~7，將放入其它 3 隻小怪獸的程式，按下部署後即可追蹤 4 隻小怪獸，並顯示座標位置。

    <img src="https://md.webduino.io/uploads/upload_254d4929a77ea282371f5cf89b10a34b.png" alt="" width="">

    > 因為程式設計方式，所以同時追蹤 4 隻小怪獸時只會顯示綠色小怪獸的資訊。

