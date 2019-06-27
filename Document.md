## Node.js 及 NPM
- Node.js 官網 : https://nodejs.org

## 介紹
- nodejs的LINE Messaging API SDK使用LINE Messaging API輕鬆開發機器人，您可以在幾分鐘內創建一個樣本機器人。
- Node.js 8或更高版本
- 對比於 PHP (程式語言) 和 Composer (相依管理工具) 之間的關係，在 Javascript 的世界裡就是 Node.js 和 NPM。由於 Node.js 的生態圈現在非常的活躍且更迭迅速，NPM 這種套件相依管理工具就變得尤其重要。因此官方在釋出安裝檔時，已經綁定 Node.js 及 NPM，在安裝時會一併安裝。

## 其他語言架設範例，請參閱以下 LINE Bot SDK repositories
- PHP : https://github.com/line/line-bot-sdk-php
- Go : https://github.com/line/line-bot-sdk-go
- Perl : https://github.com/line/line-bot-sdk-perl
- Ruby : https://github.com/line/line-bot-sdk-ruby
- Python : https://github.com/line/line-bot-sdk-python
- Node.js : https://github.com/line/line-bot-sdk-nodejs


## step 1 : 更新 Ubuntu
#### nodejs使用apt包管理器安裝：
```
# apt-get update
# apt-get install nodejs
```

#### 來自Ubuntu存儲庫的Node.js可執行文件被命名，nodejs而不是node因為與另一個包衝突。要驗證安裝，請執行以下命令：
```
# nodejs --version
```

```

```

## NPM是隨同NodeJS一起安裝的包管理工具，能解決NodeJS代碼部署上的很多問題，常見的使用場景有以下幾種：
- 允許用戶從NPM服務器下載別人編寫的第三方包到本地使用。
- 允許用戶從NPM服務器下載並安裝別人編寫的命令行程序到本地使用。
- 允許用戶將自己編寫的包或命令行程序上傳到NPM服務器供別人使用。
```
# apt-get install npm
```

#### 基本上以上的步驟已經安裝好 Node.js 及 NPM，不過因為 NPM 有時候會需要在本機端編譯一些套件，所以會建議把編譯套件 (build-essential) 也裝起來。
```
# apt-get install build-essential
```



## 參考資料
- How to install Node.js and npm on Ubuntu 18.04 : https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/
- 第 17 天：安裝 Node.js 及 NPM : https://ithelp.ithome.com.tw/articles/10194339
- LineBot+Python，輕鬆建立聊天機器人 : https://yaoandy107.github.io/line-bot-tutorial/
- Day27 關於LINE Bot 還有這些注意事項！(3) : https://ithelp.ithome.com.tw/articles/10206767


