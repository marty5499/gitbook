 

# Google 試算表

在日常生活中，有許多需要大量資料紀錄的情境，如：位置追蹤、上下班打卡、成績統計、溫度監控等等。而這些應用都可以透過使用 Google 試算表作為資料庫，配合 Web:AI 「Google 試算表」積木輕鬆達成。

## 試算表設定

使用 Web:AI 操作 Google 試算表前，需要先建立好試算表並開啟共用權限。

### 建立試算表

1. 登入 Google 帳號，進入 Google 雲端硬碟。

    <img src="https://md.webduino.io/uploads/upload_b74b1d840dc2ff167f89cbfa39b5f48c.png" alt="" width="">

2. 點擊右鍵，建立試算表。

    <img src="https://md.webduino.io/uploads/upload_f054cf6c27567ba076dc476ceb216d27.png" alt="" width="">

3. 需要設定的部分如下：

    - 共用設定：讓 Web:AI 具備編輯試算表的權限。
    - 工作表名稱：設定編輯哪一頁的工作表。

    <img src="https://md.webduino.io/uploads/upload_4bb07199bdb23ee85d866f04f2158bac.png" alt="" width="">

### 設定共用權限

1. 點擊「共用」跳出視窗，點擊「變更」。

    <img src="https://md.webduino.io/uploads/upload_f48ed632a67a15f74b9f14432d0a1f76.jpg" alt="" width="">

2. 將對象設定為「知道連結的使用者」。

    <img src="https://md.webduino.io/uploads/upload_430ae1aeaeb977557363e82543244e6a.jpg" alt="" width="">

3. 將權限設定為「編輯者」。

    <img src="https://md.webduino.io/uploads/upload_a6e24ab34d968df128d292ccae448759.jpg" alt="" width="">

4. 點擊「完成」即完成權限設定。

## 試算表初始化

「試算表初始化」積木可以設定試算表的網址和工作表名稱，在操作試算表的任何功能之前，都需要先使用「試算表初始化」積木。

<img src="https://md.webduino.io/uploads/upload_a19e2386f8bb283ec9d75439bc9ad02f.png" alt="" width="">

分別需要將試算表網址、工作表分別填入。

<img src="https://md.webduino.io/uploads/upload_36ecda6935c368276bd4a6ac0501be8b.png" alt="" width="">

## 寫入資料

「寫入資料」積木能夠將資料寫入試算表 1 次，可以選擇從欄位的最上方或最下方填入。

<img src="https://md.webduino.io/uploads/upload_25089912b19fbeabd0980dc5ea8f7030.png" alt="" width="">

點選積木前方的藍色小齒輪，可以增加寫入資料的欄位數量。

<img src="https://md.webduino.io/uploads/upload_beef253a773e0e4d9425be2973ebcdd3.gif" alt="" width="60%">

### 範例：寫入 1 筆資料

1. 組合程式積木如下：

   <img src="https://md.webduino.io/uploads/upload_f8a3fadfff78f6c076e31efddc6e110e.png" alt="" width="">

2. 按下執行，可以看到在 A 欄最上方會輸入 1 筆資料。

    <img src="https://md.webduino.io/uploads/upload_442cc7323651470e13935da16a1a86eb.png" alt="" width="">


### 範例：不斷往上寫入資料

1. 組合程式積木如下：

    <img src="https://md.webduino.io/uploads/upload_64b8a16da1d0a3a0927b35b95a8afe0d.png" alt="" width="">

2. 按下執行，可以看到會從 A 欄最上方不斷輸入資料。

    <img src="https://md.webduino.io/uploads/upload_c68a3b38a3b848616946031b9f676799.png" alt="" width="">


## 指定儲存格寫入資料

「指定儲存格寫入資料」積木可以將資料寫入指定的儲存格，格式除了單一數值，也支援二維陣列格式的資料。

<img src="https://md.webduino.io/uploads/upload_662ce9bff9e31994767df5a2cb23d37d.png" alt="" width="">

- ### 寫入一維資料

    如下程式，會在「C2」輸寫入「Web:AI」。

    <img src="https://md.webduino.io/uploads/upload_5ee5abb97d6ca5a892ea9ebcdecb33b9.jpg" alt="" width="">

    <img src="https://md.webduino.io/uploads/upload_968c3963b12f42ec35c705c2daff10c3.png" alt="" width="">

- ### 寫入二維資料

    1. 指定儲存格範圍「A1:C2」。

       <img src="https://md.webduino.io/uploads/upload_c2fd3d743ece6684c5ebe78f536ed6c6.png" alt="" width="">

        <img src="https://md.webduino.io/uploads/upload_8039413aad4dc39068884708cbb7f285.jpg" alt="" width="">

    2. 使用「陣列」積木設定要輸入的資料。

         <img src="https://md.webduino.io/uploads/upload_13a2a438776e60b199c4ac64afeaa23e.png" alt="" width="">

    3. 執行後可以看到分別填入各自的資料。

        <img src="https://md.webduino.io/uploads/upload_6fc0c005c785ad5f3d61cb5492462efa.png" alt="" width="">

## 儲存格的資料

「儲存格的資料」積木能夠讀取儲存格中的資料，並將資料顯示出來。

<img src="https://md.webduino.io/uploads/upload_3b0f88ae88cbc1ac0b7cee872a57e2f6.png" alt="" width="">

### 範例：讀取 C2 的水果

1. 先將試算表填好水果資料。

    <img src="https://md.webduino.io/uploads/upload_4d1af8885b401bfb1a2315df294ba5e7.png" alt="" width="">

2. 組合積木如下，讓小怪獸說出「C2」的資料。

<img src="https://md.webduino.io/uploads/upload_a8af4a5d0f110824807eccc08914928b.png" alt="" width="">


3. 執行後，可以看到網頁互動區的綠色小怪獸說出「蓮霧」。

    <img src="https://md.webduino.io/uploads/upload_9aad3e647abe2e692a6463dd1155c4e0.png" alt="" width="">

## 最後一列 ( 欄 ) 的編號

「最後一列 ( 欄 ) 的編號」積木能夠讀取表格中的最後一列 ( 欄 ) 的編號，並將資料顯示出來。

- 列：1 2 3 4 ...
- 欄：A B C D ...

<img src="https://md.webduino.io/uploads/upload_78d1090110f1bb67558bde95526b990b.png" alt="" width="">

### 範例：讀取最後一列水果的編號

1. 先將試算表填好水果資料。

    <img src="https://md.webduino.io/uploads/upload_4d1af8885b401bfb1a2315df294ba5e7.png" alt="" width="">
 
2. 組合積木如下，讓小怪獸說出「最後一列水果的編號」的資料。

    <img src="https://md.webduino.io/uploads/upload_7102791fb4e856f9146e33091c33dda4.png" alt="" width="">

3. 執行後，可以看到網頁互動區的綠色小怪獸說出「2」。

    <img src="https://md.webduino.io/uploads/upload_4b509906f7e00e104373857a393a2c26.png" alt="" width="">

## 刪除列 ( 欄 )

「刪除列 ( 欄 )」積木可以刪除一個區間的列或欄。

- 列：1 2 3 4 ...
- 欄：A B C D ...

<img src="https://md.webduino.io/uploads/upload_adb4eabdddf2e258f59b8e25db439685.png" alt="" width="">

### 範例：刪除 A 欄

1. 先將試算表設定如下：

    <img src="https://md.webduino.io/uploads/upload_7bf8cb1f981f862a07c60199eadb486d.png" alt="" width="">


2. 組合程式，設定「第 A 欄到第 A 欄」，代表刪除第「A」欄。

    <img src="https://md.webduino.io/uploads/upload_891d753ecabbf1ffbd3058e07ba6573f.png" alt="" width="">

3. 執行後可以看到原本的「A 欄」被清掉，只剩下原本的「B 欄」、「C 欄」。

    <img src="https://md.webduino.io/uploads/upload_a2f8726c1d77016e70682564089ae0d3.png" alt="" width="">

## 增加列 ( 欄 )

「增加列 ( 欄 )」積木可以增加一個區間的列或欄。

- 列：1 2 3 4 ...
- 欄：A B C D ...

<img src="https://md.webduino.io/uploads/upload_42edbd7120ed6e8377665af798fe4751.png" alt="" width="">

### 範例：增加 A 欄

1. 先將試算表設定如下：

    <img src="https://md.webduino.io/uploads/upload_7bf8cb1f981f862a07c60199eadb486d.png" alt="" width="">


2. 組合程式，設定「第 A 欄的左邊增加 1 欄」。

    <img src="https://md.webduino.io/uploads/upload_a3a62d659afa6f4ee4e362cea5216951.png" alt="" width="">

3. 執行後可以看到原本的「A 欄」左側增加 1 欄，原本的資料全部往右平移。

    <img src="https://md.webduino.io/uploads/upload_52e474ca7567edbba6413939f821e7da.png" alt="" width="">
