#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md) / [`Web:AI MoonCar`](./`Web_AI MoonCar`_WL73SmMMQN-Aw217YB_Z3g.md)

# 顏色感測

MoonCar 車底下配置了白色 LED 補光燈及顏色感測器，使用顏色感測時，白色 LED 補光燈會向下發光，透過顏色感測器來偵測反射的光線顏色。

可以使用 Web:AI MoonCar 附贈的 9 張顏色偵測色卡，讓小車偵測並執行不同的程式情境。

<img src="https://md.webduino.io/uploads/upload_2510bd427da3008a23ba3b725616415f.png" alt="" width="400">

## 顏色感測積木

「顏色感測」積木代表偵測到的地板顏色，回傳的值為「是」或「否」。

搭配「無限重複」積木可以不斷偵測。

<img src="https://md.webduino.io/uploads/upload_da54f2583f116a3186cc7e30807ef335.png" alt="" width="">

## 範例：回報偵測到的顏色

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 先設定小車的速度及前進方向。

    <img src="https://md.webduino.io/uploads/upload_5cf35cff29135c7173d8680fdad8cc36.png" alt="" width="">

2. 使用「邏輯判斷」積木，當偵測到「深藍色」時，綠色小怪獸會說「深藍色」。

    <img src="https://md.webduino.io/uploads/upload_4137fb1ad59e13bf061e8a13d5c97df1.png" alt="" width="">

3. 增加其它顏色，讓小車偵測到不同顏色時，綠色小怪獸會說不同顏色。

    <img src="https://md.webduino.io/uploads/upload_e8d9f5732a4cf76cdb682dbbcf4567a4.png" alt="" width="">

4. 加入「無限重複」積木，讓顏色偵測可以不斷執行。

    <img src="https://md.webduino.io/uploads/upload_8cab7a53ca67420adf0bb69f23f6ebe4.png" alt="" width="">

5. 完成後點擊執行，小車會開始前進，將顏色偵測色卡放在小車行進的路線上，綠色小怪獸說出現在地板的顏色。

    <img src="https://md.webduino.io/uploads/upload_516e29520755738909c6a06b3fe6f71a.png" alt="" width="">

## 範例：循跡紅色停止

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 現在地面貼上黑色膠帶，製作小車行駛的軌跡，並放上紅色色卡，代表小車到這裡會停止。

2. 設定小車速度及循跡方式。

    <img src="https://md.webduino.io/uploads/upload_d4a4c7802a806a9e8ffdb65ae3c84d6c.png" alt="" width="">

3. 使用「邏輯判斷」積木，讓小車偵測到紅色會停止和停止循跡。

    <img src="https://md.webduino.io/uploads/upload_9307e6c3a152efdba5747df7cbef9f8b.png" alt="" width="">

4. 在後面加入「否則」，沒偵測到紅色時會繼續啟動循跡。

    <img src="https://md.webduino.io/uploads/upload_573d868d9a7378b3cdfc41ff96f0f122.png" alt="" width="">

5. 加入「無限重複」積木，讓顏色偵測可以不斷執行。

    <img src="https://md.webduino.io/uploads/upload_eac93f5823942e7ae63a60461fb0c039.png" alt="" width="">

6. 完成後按下執行，就可以讓小車在黑色膠帶上行駛，到達紅色色卡時會停止，移開色卡後會繼續循跡。

    <img src="https://md.webduino.io/uploads/upload_fec955ab0baaaa86ba4254008fed5e65.png" alt="" width="">
