#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md) / [`Web:AI MoonCar`](./`Web_AI MoonCar`_WL73SmMMQN-Aw217YB_Z3g.md)

# 循跡自走

Web:AI MoonCar 底盤前方具備了兩個 IR 循線感測器，只要將黑色膠帶貼在地面，並使用簡單的幾塊積木，就可以讓 MoonCar 快速達成循跡自動駕駛功能。

<img src="https://md.webduino.io/uploads/upload_359799094bef6b05ee5eccfffaf10160.jpg" alt="" width="550">

## 循跡原理

MoonCar IR 循線感測器會向下發出垂直地面的紅外線 ( IR )，當紅外線照射到路面及黑色物體時，會產生不同的反射結果，根據偵測反射的結果來控制小車的動作。

- 偵測地面：紅外線被反射 → 感測器偵測到反射的紅外線 → LED 不亮
- 偵測黑色膠帶：紅外線被吸收 → 感測器偵測未偵測紅外線反射 → LED 亮綠燈

<img src="https://md.webduino.io/uploads/upload_38c691d7c27fa4c0a66509e72e40a954.png" alt="" width="">

## 循跡設定

「循跡設定」積木可以依照 IR 循線感測器偵測的結果來做方向控制，IR 循線感測器訊號分為：

- ○○：無黑線
- ○●：右感測器有黑線
- ●○：左感測器有黑線
- ●●：左右感測器皆有黑線

> 有偵測到黑色膠帶會亮綠燈指示，積木為 ●。
> 未偵測到黑色膠帶不會亮燈，積木為 ○。

一般情境使用設定會如下：

<img src="https://md.webduino.io/uploads/upload_ecd5e26123b27176815d979661d93f43.png" alt="" width="">

<img src="https://md.webduino.io/uploads/upload_89cb4105366acedcab28cc4487e99038.png" alt="" width="">

### 範例：基本循跡自走

只需要使用 3 塊積木，就能讓 Web:AI MoonCar 開始循跡自走！

#### ➤ 前往 [`範例連結`](./`範例連結`_.md)

1. 設定 MoonCar 的速度。

    <img src="https://md.webduino.io/uploads/upload_13c5385fc7eaef21c6c6cb5cc5e01751.png" alt="" width="">


2. 使用「循跡設定」積木，執行後即可開始基本循跡自走。

    <img src="https://md.webduino.io/uploads/upload_db931b67ab63cf48c9d37dd3cfdc6b45.png" alt="" width="">

3. 也可以另外放入「小怪獸說話」積木，將 MoonCar 的運作情形顯示在網頁互動區上。

    <img src="https://md.webduino.io/uploads/upload_ce5f2c46e78e34e2108a81ecc0a0a4bc.png" alt="" width="">

> 循跡功能會受到膠帶軌跡、車速快慢、小車電量影響，循跡不順時可以調整這 3 個條件來達到最好的循跡效果。

## 啟動 ( 停止 ) 循跡

除了設定循跡外，更可以使用「啟動循跡」和「停止循跡」積木來控制啟動和停止。

<img src="https://md.webduino.io/uploads/upload_f8b1e16a374a0e720d53920aed33e35a.png" alt="" width="">

### 範例：小怪獸循跡開關

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 首先設定初始速度及設定循跡。

    <img src="https://md.webduino.io/uploads/upload_8af099212bf083910490b1efe85d76e6.png" alt="" width="">


2. 使用「滑鼠點擊小怪獸」積木，分別放入「啟動循跡」和「停止循跡」積木，作為循跡的開關。

    - 綠色小怪獸：啟動循跡
    - 紅色小怪獸：停止循跡

    <img src="https://md.webduino.io/uploads/upload_dc98e81c103533e4dfc2e1dc747779da.png" alt="" width="">

3. 加入「小怪獸說話」積木和「LCD 畫文字」積木標示。
   開始執行後，就可以使用紅綠小怪獸來控制循跡了。

    <img src="https://md.webduino.io/uploads/upload_f5b50f9252d1ec0e7f34c6ac33649f36.png" alt="" width="">

## 進階範例：小怪獸物件追蹤控制小車

結合小怪獸物件追蹤控制 MoonCar，偵測不同的小怪獸來執行相對應的動作。

> 關於物件追蹤積木，歡迎參考：[物件追蹤](./物件追蹤_GGYamCnETxeO1KByVciVbA.md)。

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 首先設定物件追蹤模型、車速以及循跡，範例使用內建的小怪獸模型。

    <img src="https://md.webduino.io/uploads/upload_5eecdc4a1c077e6ac582eba35d062faf.png" alt="" width="">

2. 放入「無限重複」積木及「開始偵測物件」積木，讓 Web:AI 可以不斷偵測。

    <img src="https://md.webduino.io/uploads/upload_8de8d83c7e0e1d3f885b6d11b067b599.png" alt="" width="">

3. 設定物件追蹤及「邏輯」積木，當偵測到綠色小怪獸時，會啟動循跡及前進。

    - greenGroup：偵測到的所有綠色小怪獸。

    <img src="https://md.webduino.io/uploads/upload_85fd67fbcaedb4b96303e34068bcb5b5.png" alt="" width="">

4. 接著設定紅色小怪獸，當偵測到紅色小怪獸時，MoonCar 會停止及停止循跡。

    - redGroup：偵測到的所有紅色小怪獸。

    <img src="https://md.webduino.io/uploads/upload_1b30209bf061dd2ae215ae050e793071.png" alt="" width="">

4. 完成後按下執行，就可以使用物件追蹤紅綠小怪獸來控制 MoonCar 的動作了。
