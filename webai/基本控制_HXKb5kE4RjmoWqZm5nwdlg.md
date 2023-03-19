#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md) / [`Web:AI MoonCar`](./`Web_AI MoonCar`_WL73SmMMQN-Aw217YB_Z3g.md)

# 基本控制

MoonCar 具備最基本遙控車的控制方式，包含方向、速度，可以配合其它積木來自由操控遙控車。加上 Web:AI 的影像辨識功能，可以輕易做出自動駕駛的應用。

## 自動車動作

「自動車動作」積木能夠控制 MoonCar 移動，包含各方向及前進停止。

<img src="https://md.webduino.io/uploads/upload_2160e84a34bfd2263de7bea7f6e803c2.png" alt="" width="">

## 自動車速度

「自動車速度」積木可以分別對左右輪、兩輪設定速度。

<img src="https://md.webduino.io/uploads/upload_12a871c2eb544be20613fde730950051.png" alt="" width="">

## 範例：正方形路徑

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用積木如下，讓 MoonCar 前進 3 秒後原地左轉，用「函式」積木組合。

    <img src="https://md.webduino.io/uploads/upload_d791d9c59c40f18a7dd7c83155d65f4e.png" alt="" width="">

2. 將函式重複 4 次，即可讓 MoonCar 行駛正方形的路徑，最後停在起點。

    <img src="https://md.webduino.io/uploads/upload_258fa619d40ac096ec01391fe1e4edf7.png" alt="" width="">

## 範例：小怪獸控制速度

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 設定 MoonCar 的預設速度和動作，讓 MoonCar 可以不斷往右前行走。

    > 因為改變速度後需要重新觸發動作，因此會在後面使用「無限重複」積木讓 MoonCar 能夠重複觸發動作「右前」。

    <img src="https://md.webduino.io/uploads/upload_2e098cf7559c8bdce0ed2eccf3ca2f61.png" alt="" width="">

2. 放入「滑鼠點擊小怪獸」積木設定不同的車速，讓 MoonCar 可以透過點擊小怪獸來控制車速。

    <img src="https://md.webduino.io/uploads/upload_e0aaeb49ba79d61a6303512e2c3d47bf.png" alt="" width="">


3. 加入「小怪獸說話」積木，設定為對應速度的文字。
   執行後，就可以分別點擊小怪獸來控制對應的速度。

    <img src="https://md.webduino.io/uploads/upload_ce52783d0762df01f6d1d105416b0b55.png" alt="" width="">

## 範例：鍵盤遙控車

使用「鍵盤偵測」積木來控制 MoonCar 吧！

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 設定 MoonCar 的起始速度。

<img src="https://md.webduino.io/uploads/upload_79cd7d0caa767559ef0431725e16b251.png" alt="" width="">

2. 使用「鍵盤偵測」積木，分別設定如下：

    - 上：前進
    - 下：後退
    - 左：原地左轉
    - 右：原地右轉
    - 空白鍵：停止

    <img src="https://md.webduino.io/uploads/upload_1dc223405df050197d1814d2b9ab457f.png" alt="" width="">

3. 開始執行後，就可以使用鍵盤方向鍵遠端控制 MoonCar 了。

## 範例：鍵盤遙控車拍照

#### ➤ 前往 [`範例連結`](./`範例連結`_.md)

1. 接續 [範例：鍵盤遙控車](https://md.webduino.ioundefined)，完成用鍵盤控制遙控車程式。

    <img src="https://md.webduino.io/uploads/upload_3fe5bd40fcf0e0d00588618900de1f7b.png" alt="" width="">

2. 增加「鍵盤偵測」積木，當按下「enter」時，會拍照上傳雲端，並使用綠色小怪獸展示照片。

    <img src="https://md.webduino.io/uploads/upload_4e92e9d5601246dec63cd5b23345fb6e.png" alt="" width="">

3. 使用「無限重複」積木配合「LCD 顯示圖片」積木，讓 Web:AI 螢幕顯示鏡頭現在拍到的畫面。

    <img src="https://md.webduino.io/uploads/upload_caf4bcb53831bba20b88a8cc4b727752.png" alt="" width="">

4. 執行後，可以用方向鍵控制小車前後左右，並且按下「enter」拍照並使用綠色小怪獸顯示出來。

    <img src="https://md.webduino.io/uploads/upload_723ec41d4e6a39f1431978ee45d16353.png" alt="" width="">
