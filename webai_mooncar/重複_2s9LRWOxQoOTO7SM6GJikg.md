 

# 重複

在程式領域裡，重複 ( 迴圈 ) 是常常使用的基本功能，能夠控制重複執行的過程，也可以將需要重複執行的程式碼放在重複內，就能指定次數、延遲時間，或是無窮盡的執行。

## 等待

「等待」積木可以讓程式暫停一段時間，當程式積木執行到「等待」積木，就會等待指定的時間過後才會進行接續的動作。

<img src="https://md.webduino.io/uploads/upload_14051453cdcb767d80b160b5ad1b10b6.png" alt="" width="">


### 範例：文字閃爍

下方的範例讓 Web:AI 的螢幕中的文字每秒顏色閃爍。

<img src="https://md.webduino.io/uploads/upload_48343e9596b015ec712d86a3cf15a0db.gif" alt="" width="">

## 重複 ( 重複幾次、無限重複次 )

「重複」積木分為「重複幾次」積木及「無限重複次」積木，功能分別如下：

- 「重複幾次」積木：指定重複內的積木程式重複的次數，預設次數為 10 次。
- 「無限重複次」積木：無止盡的執行重複內容，除非使用「中斷循環」積木，重複的事件才會停止。

<img src="https://md.webduino.io/uploads/upload_acc38cc8518f6a375cdfba2208b5a3d1.png" alt="" width="">

### 範例：文字閃爍 10 次

1. 以相同的文字顏色閃爍為例，將「無限重複」積木替換成「重複 10 次」積木，按下執行，可以看到 Web:AI 螢幕顯示 Webduino 文字顏色閃爍。  
2. 當執行完第 10 次後，會停止執行程式，Webduino 的文字顏色停留在紅色不再改變。

   <img src="https://md.webduino.io/uploads/upload_263b347ab87292fd9a6dde4c4f08d4c4.png" alt="" width="">

## 判斷為真，就重複無限次

「判斷為真，就重複無限次」積木等同於「重複無限次」積木加上「邏輯」判斷，只要空格內的邏輯判斷為「真」( true )，就會開始進行無限重複。

<img src="https://md.webduino.io/uploads/upload_67d738e94f23852ac2a2d983b2dc07aa.png" alt="" width="">

### 範例：隨機取數，是偶數就停止

1. 設定一變數「number」為 1~100 隨機數字，如果 number 是偶數時，就重複後續動作無限次。

   <img src="https://md.webduino.io/uploads/upload_b2765fc857de3a37590e42d42b723222.png" alt="" width="">

2. 完成積木後按下執行，可以在 Web:AI 螢幕看到 number 的取得的數值。

    - 如果 number 為奇數，螢幕顯示白色數字
    - 如果 number 為偶數，螢幕顯示數字顏色不斷閃爍。

   <img src="https://md.webduino.io/uploads/upload_ddbde1a3a7c675073e1bfd80a36f492d.png" alt="" width="">

## 計數

「計數」積木類似「重複執行幾次」積木，差別在於計數積木使用了一個變數 ( i )，透過改變這個變數的數值，來決定重複幾次、如何重複以及重複的間隔。

> 以預設的「計數」積木為例，「變數 i」的數值會由 1 , 2 , 3 , ... , 10 的方式改變。

<img src="https://md.webduino.io/uploads/upload_8d06b1db227a0a01349f10e31d233aff.png" alt="" width="">

### 範例：依序顯示 1 , 2 , 3 , ...... , 10

在「LCD 顯示文字」積木內放入「變數 i」積木，讓 Web:AI 螢幕顯示 i 的數值，並且設定「等待 1 秒」，按下執行，可以看到螢幕顯示 1 , 2 , 3 , … , 10。

<img src="https://md.webduino.io/uploads/upload_d5d81e32c4195fc8c5c3750af633b00a.gif" alt="" width="">

## 取出陣列元素並執行

「取出陣列元素並執行」積木是以陣列長度作為重複次數的依據，因此空格內必須放入陣列積木，執行後就會依序取出陣列內容並執行對應動作。

<img src="https://md.webduino.io/uploads/upload_b4b8436236ed918a0f343c316de11985.png" alt="" width="">


### 範例：依序顯示 A B C

使用「陣列」積木建立列表，放入「文字」積木 A、B、C，「變數 i」代表列表中的每一個項目，設定讓 LCD 顯示「變數 i」，按下執行，就可以看到 Web:Bit 螢幕依序顯示 A、B、C。

<img src="https://md.webduino.io/uploads/upload_5725ac932f2eedf1774358b8a16fb75d.gif" alt="" width="">

## 停止這個重複

在重複的過程中，可以使用「停止這個重複」積木來終止目前的循環。

<img src="https://md.webduino.io/uploads/upload_2d3eaf4cf2ec60ff58993948eeca005d.png" alt="" width="">


### 範例：數到 20 就停止

下方範例是 Web:AI 螢幕顯示從 1 數到 50，當「變數 i」= 20 時會停止循環，所以螢幕上的數字會停在 20。

<img src="https://md.webduino.io/uploads/upload_41ad4328cc597d1ca61cfda7aab53e35.png" alt="" width="">
