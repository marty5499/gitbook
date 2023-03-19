#### 回到 [`教學大綱`](./`教學大綱`_qo4Ew_UQTU25aAm8DfFHFw.md) / [`Web:AI MoonCar`](./`Web_AI MoonCar`_WL73SmMMQN-Aw217YB_Z3g.md)

# 感測器 & 控制器

MoonCar 除了馬達控制外，還配置了按鈕、超音波感測器、紅外線控制、蜂鳴器等感測控制器。透過這些功能，就可以用最簡單的方式完成物聯網操控 MoonCar。

## 小車按鈕

小車後方一顆按鈕開關，當按下小車按鈕時，會觸發後續的動作。
觸發方式分為：
- 按下
- 放開
- 長按

<img src="https://md.webduino.io/uploads/upload_eb6b476156083441055e3a6d4d1b482c.png" alt="" width="">

### 範例：小車按鈕開燈

使用小車按鈕點亮 8 顆 LED 燈。

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用「小車按鈕」積木，設定為「按下」及「開啟」狀態。

    <img src="https://md.webduino.io/uploads/upload_3f34c52d0d5e92e769087da6d3a36a1c.png" alt="" width="">

2. 使用「循環計數」積木，設定讓第 1 ~ 8 顆 LED 燈亮起橘色燈。

    <img src="https://md.webduino.io/uploads/upload_04eea0778960c843beb87da7f40e6660.png" alt="" width="">

3. 加入「關閉魔幻 LED」積木，讓按鈕放開時，會關閉 LED 燈。

    <img src="https://md.webduino.io/uploads/upload_a84b1c0319ba806c85b76b0ea2d92f6e.png" alt="" width="">

4. 執行後，可以按下 MoonCar 按鈕就可以控制 LED 燈亮起熄滅了。

## 超音波感測

Web:AI MoonCar 附贈了像眼睛一樣的超音波感測器，透過超音波的反射可以計算出和前方物體的距離，進而做出車距控制系統以及緊急煞車輔助系統。

<img src="https://md.webduino.io/uploads/upload_66678e50b4a4113476c5d57105f3e9ec.png" alt="" width="">

### 原理

超音波感測器會向前發射超音波，碰到物體後會反射回來，接收到反射的超音波後，根據發射反射的時間差計算出和物體之間的距離。

> 因為超音波具有指向性，若感測的物體是傾斜、不規則形狀或是材質容易吸收超音波，會導致測量距離不準確。
>- 傾斜、不規則形狀：超音波容易漫反射。
>- 材質容易吸收超音波：超音波反射減少。

<img src="https://md.webduino.io/uploads/upload_d401ca6891a2af12f12d1f89942487cc.jpg" alt="" width="">

### 安裝超音波感測器

在小車前方有 2 排插槽，分別是超音波插槽及 I2C 擴充插槽，將超音波感測器插入「**前排**」插槽，就可以開始使用。

> 若誤將超音波感測器插在後排插槽，可能會導致感測器損壞，請小心使用！

<img src="https://md.webduino.io/uploads/upload_26545126851308206f6c020e08d97543.jpg" alt="" width="">

### 超音波積木

「超音波」積木可以直接達成發射接收超音波、計算距離的功能，配合其它積木可以做出控制行車距離的效果。

<img src="https://md.webduino.io/uploads/upload_69aa6adf5290d3487f41d616762c7ea8.png" alt="" width="">

### 範例：超音波感測

1. 使用「小怪獸說話」積木說出「超音波」積木的數值，並且配合「無限重複」積木讓小車可以不斷感測。

    <img src="https://md.webduino.io/uploads/upload_439115ca9e02026f94aac8854320d5fa.png" alt="" width="">

2. 執行後，用手或物體在超音波前移動，可以看到超音波數值不斷變化。

    <img src="https://md.webduino.io/uploads/upload_29479b5e46a01754d9af81cbc8e47fae.gif" alt="" width="">

### 範例：車距控制系統

#### ➤ 前往 [`範例連結`](./`範例連結`_.md)

1. 先決定好行車距離，如範例為 20 公分，小車的行動規則如下：
    - 車距 = 20 公分：停止
    - 車距 < 20 公分：後退
    - 車距 > 20 公分：前進

    <img src="https://md.webduino.io/uploads/upload_6f81ee3563d297ceadb275643ee121fa.png" alt="" width="">

2. 在外層加上「無限重複」積木，讓超音波重複感測。

    <img src="https://md.webduino.io/uploads/upload_8c31c516ed332a28cc6aaec7eea76eae.png" alt="" width="">

3. 最後在程式開始前設定車速。
   執行後，用手或物體在超音波前移動，可以看到小車會和前方物體會保持一定的距離。

    <img src="https://md.webduino.io/uploads/upload_7f4c8619f5deee77dd22603fb10113e9.png" alt="" width="">

## 紅外線

日常各種電器都會使用紅外線，MoonCar 具備接收和發射的功能，可以接收遙控器的紅外線訊號，也可以對電器發射訊號。

### 紅外線接收

<img src="https://md.webduino.io/uploads/upload_7ce29a2b1476acbb6fe4b862652dad09.png" alt="" width="">

### 紅外線發射

<img src="https://md.webduino.io/uploads/upload_14ea651eafb0134eab64577c68b276d1.png" alt="" width="">

### 範例：接收紅外線訊號

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 組合積木如下：

    <img src="https://md.webduino.io/uploads/upload_27894b0cdbc740166065e6b56abb3988.png" alt="" width="">

2. 執行後，對著小車發送紅外線，就可以看到綠色小怪獸顯示紅外線訊號代碼。

    <img src="https://md.webduino.io/uploads/upload_e042df147f1c45da51450cdbb53de1cb.png" alt="" width="">

### 範例：紅外線遙控 MoonCar

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用「邏輯」積木，當紅外線接收的代碼 = 特定數字時，會執行後續動作。

    > 代碼數值不同設備的紅外線訊號會不一樣，需要自行設定接收的代碼。

    <img src="https://md.webduino.io/uploads/upload_63f6ad24e74e631b49f30ff59f8e83b6.png" alt="" width="">

2. 組合積木如下，接收到訊號時會控制不同的 LED 燈亮起。

    <img src="https://md.webduino.io/uploads/upload_c06580a0468102827c08ec6b3ffb3f55.png" alt="" width="">

### 範例：發射紅外線訊號

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 設定要發送的紅外線訊號，如範例設定代碼為 00FF22DD。

    <img src="https://md.webduino.io/uploads/upload_9352793f3a2e98df0ad47ddaef6fce6f.png" alt="" width="">

2. 設定觸發方式，點擊小怪獸後會發射紅外線。
   執行後，就可以點擊小怪獸發射紅外線了。

    <img src="https://md.webduino.io/uploads/upload_c4124ef1a4538e3cc20b09e951323caa.png" alt="" width="">

## 蜂鳴器

MoonCar 配置了蜂鳴器的功能，可以在不接上喇叭的情境下就能做出音效。
可以設定聲音頻率及持續時間。

<img src="https://md.webduino.io/uploads/upload_b7574e91a9098789b64a0cc17d3334ba.png" alt="" width="">

### 範例：小怪獸發聲

1. 設定點擊小怪獸，蜂鳴器會發出音效。

    <img src="https://md.webduino.io/uploads/upload_ddd558ae3a555403e6243cef544e8088.png" alt="" width="">

2. 重複 4 個，讓點擊 4 隻小怪獸分別會發出不同聲音。

    <img src="https://md.webduino.io/uploads/upload_964257facd3df37893ccdd65e062a372.png" alt="" width="">

3. 執行後，可以點擊不同小怪獸發出不同音效。
