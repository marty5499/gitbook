 

# 人臉追蹤

在 AI 人工智慧中，最重要的就是人臉識別，可以根據人臉的特徵，如：眼睛、鼻子、嘴巴、鼻子等。透過這項技術，可以偵測到是否有人經過以及畫面中的人數，進一步做出監視器等應用。

而 Web:AI 的人臉追蹤技術，可以做到追蹤人臉的座標位置，以及人臉在畫面中的寬度、高度，更配合疫情時事，增加了口罩辨識的功能，讓 AI 結合生活應用，更方便用於教學。

## 照相畫面

「拍攝照片」積木可以使用鏡頭拍攝一次畫面，配合「無限重複」積木就可以達成照相鏡頭的效果。

<img src="https://md.webduino.io/uploads/upload_e5f0e28421cf299a02c56d80badc8485.png" alt="" width="">

另外也可以使用「變數」積木替拍攝照片命名，透過命名來做出更多變化。

<img src="https://md.webduino.io/uploads/upload_2630972dadc38129eb09e64e7d262658.png" alt="" width="">

> 以上兩種積木組合方式執行後會達到相同的結果，差別在於若是要做出更多應用變化，就需要搭配「變數」積木的命名。

### 畫面上畫文字

Web:AI 能夠在螢幕畫面或圖片上顯示文字，這時就需要搭配「圖片上畫文字」積木。

> 請特別注意，「圖片上畫文字」積木需要放在「LCD 顯示圖片」積木之前！

<img src="https://md.webduino.io/uploads/upload_d4fc3f4eca1a16281c9aade6bb111715.png" alt="" width="">

## 鏡頭反轉

「鏡頭反轉」積木能夠將 Web:AI 鏡頭翻轉。

<img src="https://md.webduino.io/uploads/upload_2763326c22227fa00047cd26a391341e.png" alt="" width="">

必須放置在程式開始處，才能讓顯示畫面翻轉。

<img src="https://md.webduino.io/uploads/upload_3f75f6bd07c715fad3e9c806c6ff7e2c.png" alt="" width="">

## 取得圖片的人臉資訊

「取得圖片的人臉資訊」積木能夠在畫面中判斷人臉特徵，並將偵測到的人臉用白框框起來。

<img src="https://md.webduino.io/uploads/upload_deef20fc56ca67c2a61f0dff7ffa4865.png" alt="" width="">

## 取得人臉資訊

「取得人臉資訊」積木代表從鏡頭中的人臉讀取到的資訊，包含位置 ( x 座標、y 座標 )及大小 ( 寬度、高度 )。

<img src="https://md.webduino.io/uploads/upload_300c4b47308ba5100134338d8f53ce3e.png" alt="" width="">

## 判斷人臉有無戴口罩

讀取到畫面的人臉後，可以進一步判斷是否配戴口罩，透過「判斷人臉有無戴口罩」積木，可以針對人臉是否戴著口罩回傳「是」或「否」，更能做出口罩偵測機的應用。

<img src="https://md.webduino.io/uploads/upload_bb7707e5b01fea74606915bc5f4cd6a7.png" alt="" width="">

## 範例：追蹤人臉座標

1. 先使用「變數」積木將拍攝照片命名為「畫面」，做出鏡頭畫面。

   <img src="https://md.webduino.io/uploads/upload_f345072205d970e61952b802116f042a.png" alt="" width="">

2. 使用「變數」積木，將「取得圖片的人臉資訊」積木命名為「人臉資訊」。
    現在執行後可以在畫面中框出人臉。

    <img src="https://md.webduino.io/uploads/upload_396fb589d4157779453859ca5fe4c8e2.png" alt="" width="">

3. 使用「圖片上畫文字」積木，放入「文字」積木，做出人臉的 xy 座標。

   <img src="https://md.webduino.io/uploads/upload_b96f96011107dd369cc944a6705d8edc.png" alt="" width="">

4. 按下執行，可以看到開始追蹤人臉，並同步顯示人臉的位置座標。

## 範例：口罩偵測器

1. 先使用「變數」積木將拍攝照片命名為「畫面」，做出鏡頭畫面。

    <img src="https://md.webduino.io/uploads/upload_f345072205d970e61952b802116f042a.png" alt="" width="">

2. 使用「變數」積木，將「取得圖片的人臉資訊」積木命名為「人臉資訊」。
    現在執行後可以在畫面中框出人臉。

    <img src="https://md.webduino.io/uploads/upload_396fb589d4157779453859ca5fe4c8e2.png" alt="" width="">

3. 使用「圖片上畫文字」積木，放入「文字」積木，顯示「口罩偵測中...」。

    <img src="https://md.webduino.io/uploads/upload_ca1d491ec5330d6f497741e0a5d1cda9.png" alt="" width="">
 
4. 在這裡加入「邏輯」積木，用來判斷人臉是否配戴口罩。
    - 配戴口罩 = 真
    - 配戴口罩 = 假 

    <img src="https://md.webduino.io/uploads/upload_8ce4a924ea5ece392c3c0e5f025cf75b.png" alt="" width="">

5. 在「邏輯」積木後放入後續要執行的動作，如：
    - 配戴口罩 = 真：顯示綠色「安全」
    - 配戴口罩 = 假：顯示紅色「警告！」

    <img src="https://md.webduino.io/uploads/upload_80741458ce4b6175eeb718ce5cf239d1.png" alt="" width="">

6. 按下執行後，就能夠開始進行口罩辨識。
可以看到沒配戴口罩時，螢幕顯示紅色「警告！」，配戴著口罩時，螢幕顯示綠色「安全」。
