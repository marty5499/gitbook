 

# LINE 

LINE 官方開發資源提供了 Noitfy 及 Chat  功能，而 Web:AI 支援了這 2 種控制方式，能夠透過聊天的方式操控 Web:AI 開發板或和小怪獸進行互動。

## Notify 及 Chat 的差異

服務名稱  | 啟用方式|推播方式|推播管道|
:-------:|:-----:|:----:|:---:|
Notify  |開通權杖 |主動傳訊|權杖|
Chat    |QR Code 加入好友 |被動回覆|頻道|


## 設定 LINE Notify

「LINE Notify」積木可以透過 LINE Notify 的服務，開通權杖 ( Token )，讓 Web:AI 主動傳訊息至 LINE 帳號中，可用來結合通知、警告等應用。

<img src="https://md.webduino.io/uploads/upload_720c391f9d6c413c0fa7e4f6b04b170f.png" alt="" width="">

### 步驟：

1. 準備好自己的 LINE 帳號密碼。

2. 前往 [LINE Notify 官方網站](./LINE Notify 官方網站_.md)。( 請使用電腦開啟！)

3. 登入帳號。

    <img src="https://md.webduino.io/uploads/upload_f340e86433f3c7dd909048ea252f658f.jpg" alt="" width="">

4. 點擊右上角帳號，選擇選單中的「個人頁面」。

    <img src="https://md.webduino.io/uploads/upload_c658929d24ea6cf0d87d2c4e9e2a13d1.png" alt="" width="">

5. 點擊「發行權杖」。
 
   <img src="https://md.webduino.io/uploads/upload_4a38479ed6c7f15ac5565f09e0bc974d.jpg" alt="" width="">

6. 設定權杖，填寫權杖名稱、接收通知的聊天室。這裡以「透過1對1聊天接收LINE Notify的通知」為例。

    - 權杖名稱：發送訊息時，會顯示的名稱。
    - 接收通知的聊天室：要使用 Notify 的聊天室，或是個人訊息。

    <img src="https://md.webduino.io/uploads/upload_bae4b9f9ceb5a5dbe1fa9e515be52095.png" alt="" width="">

7. 按下「發行」後，會出現發行的權杖如下圖，並將權杖複製。

   > 權杖只會顯示 1 次，每次使用程式積木都需要輸入，為避免忘記，建議先將權杖記錄下來。

    <img src="https://md.webduino.io/uploads/upload_75a6de365268054ac730965e0baf07cf.png" alt="" width="">

8. 設定完成後，就可以在「已連動的服務」中看到剛剛設定的權杖了。

    <img src="https://md.webduino.io/uploads/upload_4427c67eb097fe42fdfbe60efc16e99c.png" alt="" width="">

9. 打開 LINE 應用程式，可以看到名稱為「LINE Notify」的帳號發送訊息「已發行個人存取權杖。」。

<img src="https://md.webduino.io/uploads/upload_4ca5cfdb7ecb2cc2732ecd73da57258c.png" alt="" width="50%">

## LINE Notify 積木

「LINE Notify」積木具備 Token 和訊息功能，結合其它積木可以實現更多情境應用。

- Token ( 權杖 )：輸入設定的權杖。
- 訊息：欲傳送的訊息。

<img src="https://md.webduino.io/uploads/upload_720c391f9d6c413c0fa7e4f6b04b170f.png" alt="" width="">

### 範例：發送「你好！」

1. 使用「LINE Notify」積木，在 Token 輸入權杖；在訊息輸入「你好」。

    <img src="https://md.webduino.io/uploads/upload_c542522817c1b530d4e539a044220c92.jpg" alt="" width="">

2. 按下執行，可以看到 LINE Notify 傳送「你好」。

    <img src="https://md.webduino.io/uploads/upload_a7c13253390ed8ac600198818e927fda.png" alt="" width="">


### 範例：鍵盤傳訊

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 使用「對話框」積木配合「無限重複」積木，讓網頁互動區對話框可以重複使用。

    <img src="https://md.webduino.io/uploads/upload_99b637ca7403152b7d83064147ac23a2.png" alt="" width="">

2. 加入「LINE Notify」積木，在 Token 輸入權杖；在訊息放入「輸入的文字」積木。

    <img src="https://md.webduino.io/uploads/upload_1d7fd89aaef19834e6759968b3db0db0.jpg" alt="" width="">

3. 執行後，在對話框輸入文字後就可以看到 Web:AI 自動將訊息傳至 LINE 聊天室。

    <img src="https://md.webduino.io/uploads/upload_241018634394e7effc1cd6ae0fad0912.png" alt="" width="">

### 範例：口罩偵測通知

#### ➤ 前往 [`範例連結`](./`範例連結`_ai-blockly.webduino.io.md)

1. 先點擊「範例」列表，開啟「口罩偵測」範例。

    <img src="https://md.webduino.io/uploads/upload_a3de078efcac37678671d125c4c8e311.png" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_2dbf609e618e1b11505e2a10152a17bc.png" alt="" width="">

2. 在邏輯判斷「有無戴口罩 = 假」中放入「LINE Notify」積木。

    <img src="https://md.webduino.io/uploads/upload_1e8aaf6df9204c88e5eda41ea448ebd3.jpg" alt="" width="">

3. 在 Token 輸入權杖；在訊息輸入「警告！有人沒戴口罩！」。

    <img src="https://md.webduino.io/uploads/upload_42c1907a5e2aead53ba9ff3626463920.jpg" alt="" width="">

4. 按下執行，可以看到當偵測到人臉沒有戴口罩時，會自動傳訊息到 LINE Notify 中。

    <img src="https://md.webduino.io/uploads/upload_4955e0343d933711fd0f78bc051c6644.png" alt="" width="">

## 設定 LINE Chat ( Webduino AIoT )

「LINE Chat」積木能透過「聊天」的方式，接收從 LINE 發送過來的訊息，透過訊息和 Web:AI 程式積木平台或 Web:AI 開發板互動。

<img src="https://md.webduino.io/uploads/upload_5d6059ea73c83b211c97d8ef6b17fb40.jpg" alt="" width="400">

### 加入好友 QR Code

- 使用 LINE Chat 前需要先將 **Weduino AIoT** 加入好友。

1. 開啟 LINE 掃描 QR Code 功能，掃描下方 QR Code。

<img src="https://md.webduino.io/uploads/upload_aea3d405ab17d12bc80a873d48f97dcc.png" alt="" width="">

2. 點擊「Add」將官方帳號加入好友。
 
    <img src="https://md.webduino.io/uploads/upload_e66c8a982cbe5bb546f7e1065b6b64c7.png" alt="" width="">

3. 加入好友後，開啟 LINE 應用程式，可以看到歡迎通知。

    <img src="https://md.webduino.io/uploads/upload_03c6064eb00bc54e240b30c3224ccebc.png" alt="" width="">

### LINE Chat 頻道設定

在使用「LINE Chat」積木前，需要先設定要使用的頻道，步驟如下：

1. 在聊天室輸入「help」，會回覆可使用的指令。
   輸入不同的指令，會回覆對應的結果。

   <img src="https://md.webduino.io/uploads/upload_d6b2b6d6b9e63aecab50d0552e731308.jpg" alt="" width="">

2. 在聊天室輸入「id」，Webduino AIoT 會回覆隨機英文數字，代表專屬的頻道名稱。
   將這串頻道名稱輸入在積木中，就可以使用「LINE Chat」積木了。

    <img src="https://md.webduino.io/uploads/upload_f8da412fd156a72a7ba6833c294fb84b.png" alt="" width="">

3. 另外也可以使用指令「id:名稱」，自行設定頻道名稱。

    <img src="https://md.webduino.io/uploads/upload_d891815812a272838a5615cb911b8adf.png" alt="" width="">

## LINE Chat 積木

設定完頻道名稱後，就可以使用「LINE Chat」積木接收及回覆訊息了。

<img src="https://md.webduino.io/uploads/upload_5d6059ea73c83b211c97d8ef6b17fb40.jpg" alt="" width="400">

### LINE Chat 接收訊息

使用「LINE Chat 接收訊息」積木會讓 Webduino AIoT 開始接收訊息。

當我們傳送訊息給 Webduino AIoT，就會開始執行後續動作，因此「回傳訊息」、「接收的訊息」積木都必須放在「LINE Chat 接收訊息」積木內部。

<img src="https://md.webduino.io/uploads/upload_b7a6d8ac4b323aa60f3883fd4f4168ff.png" alt="" width="">

### LINE Chat 回傳訊息

「LINE Chat 回傳訊息」積木能夠設定 Webduino AIoT 要說的話。

<img src="https://md.webduino.io/uploads/upload_5c1a786d0c2d3477135861a3f1e05a74.png" alt="" width="">

使用方式如下圖，當 Webduino AIoT 接收到訊息後，會回傳訊息。

<img src="https://md.webduino.io/uploads/upload_acdceb8c2e6a9bdb53a03c6368e0c28c.png" alt="" width="">

### LINE Chat 接收的訊息

「LINE Chat 接收的訊息」代表傳給 Webduino AIoT 的訊息，可以回傳到開發板或網頁互動區。

<img src="https://md.webduino.io/uploads/upload_c4b842c07564c82781a10830b42b3cbc.png" alt="" width="">

### 範例：回傳收到的訊息

1. 使用「LINE Chat 接收訊息」積木，輸入設定的頻道名稱。

    <img src="https://md.webduino.io/uploads/upload_ee8567b3085152e6142e4ae7c2e95957.png" alt="" width="">

2. 放入「LINE Chat 回傳訊息」及「LINE Chat 接收的訊息」積木，代表 Webduino AIoT 接受到訊息後會回覆同樣的訊息。

    <img src="https://md.webduino.io/uploads/upload_60a2498f90362736c1040ca5e6e7fc14.png" alt="" width="">

3. 執行後，對 Webduino AIoT 傳送訊息，可以看到它也會回傳相同的訊息。

    <img src="https://md.webduino.io/uploads/upload_8ef9571e59c70b81da3b983da5df1245.png" alt="" width="">

<!-- ### 範例：拍照傳至 LINE -->

## LINE 貼圖

不管是使用 LINE Notify 或是 LINE Chat 都可以傳送貼圖訊息，這時候就需要用到「LINE 貼圖」積木。

<img src="https://md.webduino.io/uploads/upload_0f5164215e83a902505ee022fff7d463.png" alt="" width="">

使用時需要按照 [LINE 貼圖清單](./LINE 貼圖清單_.md) 輸入指定的表情代號及表情主題。

- 表情代號：Sticker ID
- 表情主題：Package ID

<img src="https://md.webduino.io/uploads/upload_503e31382a5fc6a2b4312bd54789acfe.png" alt="" width="">

### 範例：LINE Notify 傳送貼圖

1. 使用「LINE Notify」積木，在 Token 輸入權杖；在訊息放入「LINE 貼圖」積木。

    <img src="https://md.webduino.io/uploads/upload_feb1c651fc9ca5f51b45a4a014a6845f.jpg" alt="" width="">

2. 輸入貼圖的表情代號、表情主題，如範例：

   - 表情代號：10855
   - 表情主題：789

    <img src="https://md.webduino.io/uploads/upload_76cf5ca69c2c622242bb2bc11fef7e20.png" alt="" width="">

3. 按下執行，可以看到 LINE Notify 送出指定的貼圖。

    <img src="https://md.webduino.io/uploads/upload_7b5aff211a6367727b77162697f70b7f.png" alt="" width="">
