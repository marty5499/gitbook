#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md) / [`Web:AI MoonCar`](./`Web_AI MoonCar`_WL73SmMMQN-Aw217YB_Z3g.md)

# 魔幻 LED

MoonCar 登月小車配置了 8 顆全彩 LED，每一顆 LED 具有獨立的編號，在使用積木時，可以根據編號來控制各個 LED 燈，做出不同的燈亮效果。

<img src="https://md.webduino.io/uploads/upload_132da585ec33b3d76a51ddd1bae23fe8.png" alt="" width="">


## 魔幻 LED 積木

<img src="https://md.webduino.io/uploads/upload_c005c21637df1a3b9873e28c68bae130.png" alt="" width="">

「魔幻 LED」積木可以選擇特定編號的 LED 燈，發出 指定顏色的光，共有 70 種顏色可以選擇。

> 顏色選擇黑色和不發光有相同的效果。

## 關閉魔幻 LED

<img src="https://md.webduino.io/uploads/upload_69c476b1fe9da43aa2be2c1e50f8fca8.png" alt="" width="">

「關閉魔幻 LED」積木可以關閉現在所有的 LED 燈。

## 範例：循環燈

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用「計數」積木，讓魔幻 LED 從第 1 顆到第 8 顆接續亮燈，時間間隔 0.1 秒。

    <img src="https://md.webduino.io/uploads/upload_cad82c17e3ed73309819765b44f11ba0.png" alt="" width="">

2. 為了做出連續燈的效果，當第 2 顆亮起時，第 1 顆要關閉，因此加入「關閉魔幻 LED 燈」積木

    > 「關閉魔幻 LED 燈」積木要放置在「魔幻 LED」積木前方，不然 LED 會馬上熄滅，而無法做出循環燈的效果。
 
    <img src="https://md.webduino.io/uploads/upload_06151d4719b34a91250751c63af9f874.png" alt="" width="">
 
3. 此時程式只能執行 1 次，只要在最外層加入「重複」積木，就可以做出循環燈了。

    <img src="https://md.webduino.io/uploads/upload_28e9aed7c8fdd59cc6d9eeac5f801e00.png" alt="" width="">

## 進階範例：辨識小怪獸控制魔幻 LED

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 設定小車的初始速度、動作及物件追蹤模型，這裡以內建小怪獸模型為例。

    <img src="https://md.webduino.io/uploads/upload_3f38e5aa2ea3b9c93702a115785bf6bd.png" alt="" width="">

2. 使用「開始偵測物件」積木配合「重複」積木，讓小車不斷偵測。

    <img src="https://md.webduino.io/uploads/upload_af823075141d0aaf48430ad115416ed1.png" alt="" width="">

3. 組裝積木如下，當偵測到綠色小怪獸時，8 顆 LED 都會發出綠光。

    <img src="https://md.webduino.io/uploads/upload_7e986f2137d7acea3e7556cd735bafc5.png" alt="" width="">

4. 重複 3 次，並分別設定：紅、黃、藍，製作出程式如下，讓小車偵測到不同小怪獸 LED 會發出不同顏色的光。

    <img src="https://md.webduino.io/uploads/upload_8014e46834c62686e65e0f55346d8d69.png" alt="" width="">

5. 完成後按下執行，小車會開啟鏡頭並前進，可以拿不同小怪獸讓小車辨識，魔幻 LED 會依照不同怪獸發出不同的顏色。

    <img src="https://md.webduino.io/uploads/upload_104ff84d7d75985ff2a51f24b71f00a3.png" alt="" width="">
