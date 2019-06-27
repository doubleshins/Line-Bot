## 1. Node.js 及 NPM
- Node.js 官網 : https://nodejs.org

- Node.js 官方現在提供兩種版本：LTS 及 Current
- LTS : Long term support ，意指是當前穩定且會長期維護的版本，在撰文的當下 Node.js 是 10.16.0 版而 NPM 是 5.5.1 版。
- Current : 則是指目前最新版，可以拿到最新的功能 (Feature)。

- 對比於 PHP (程式語言) 和 Composer (相依管理工具) 之間的關係，在 Javascript 的世界裡就是 Node.js 和 NPM

## 2. Nodejs的LINE Messaging API SDK使用LINE Messaging API輕鬆開發機器人
- Node.js 8或更高版本


## 3. 其他語言架設範例，請參閱以下 LINE Bot SDK repositories
- PHP : https://github.com/line/line-bot-sdk-php
- Go : https://github.com/line/line-bot-sdk-go
- Perl : https://github.com/line/line-bot-sdk-perl
- Ruby : https://github.com/line/line-bot-sdk-ruby
- Python : https://github.com/line/line-bot-sdk-python
- Node.js : https://github.com/line/line-bot-sdk-nodejs


## 4. 更新 Ubuntu
- nodejs使用apt包管理器安裝：
```
# apt-get update
# apt-get install nodejs
```

- 來自Ubuntu存儲庫的Node.js。要驗證安裝，請執行以下命令：
```
# nodejs --version
```
```
v8.10.0
```

- NPM是隨同NodeJS一起安裝的包管理工具，能解決NodeJS代碼部署上的很多問題，常見的使用場景有以下幾種：
- 允許用戶從NPM服務器下載別人編寫的第三方包到本地使用。
- 允許用戶從NPM服務器下載並安裝別人編寫的命令行程序到本地使用。
- 允許用戶將自己編寫的包或命令行程序上傳到NPM服務器供別人使用。
```
# apt-get install npm
```

- 鍵入以下命令驗證安裝：
```
# npm --version
```

```
3.5.2
```

## 5. 從NodeSource存儲庫安裝Node.js
- NodeSource是一家專注於提供企業級Node支持的公司，他們維護一個包含最新版本Node.js的存儲庫
- 將NodeSource簽名密鑰添加到您的系統，創建apt源存儲庫文件，安裝所有必需的包並刷新apt緩存
```
# curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
```

- 或者
```
# curl -sL https://deb.nodesource.com/setup_10.x -o nodesource_setup.sh
# bash nodesource_setup.sh
```

- 啟用NodeSource存儲庫後，鍵入以下命令安裝Node.js和npm：
```
# apt-get install -y nodejs

# nodejs --version
v10.16.0

# npm --version
6.9.0
```

- 基本上以上的步驟已經安裝好 Node.js 及 NPM，不過因為 NPM 有時候會需要在本機端編譯一些套件，所以會建議把編譯套件 (build-essential) 也裝起來。
```
# apt-get install build-essential
```

## 6. 註冊LINE Channel
- 想要建置LINE Bot首先你必須要有一個LINE Channel作為使用者跟Bot對答的帳號
- LINE Developers官方網站 : https://developers.line.biz/en/

- 1. 進入LINE Developer後點選右上角的Log in 並以你的LINE帳號登入
- 2. 輸入開發者信息
- 3. 選擇「Create New Provider」

## Provider可想像成是一個公司或是團隊層級的帳號，LINE Bot會被綁在這組Provider帳號底下

## 若我們只是想嘗試建置Bot，可輸入任何一個尚未被使用過的名稱即可

- 4. 當Provider建立好後，進入Provider的頁面內，點選「Create Channel」
- 5. 當Channel成功被建立後，在Provider list進入「Channel Settings」

## 在Channel Settings畫面裡總共有三個重要的資料要找到：
- Channel ID
- Channel Secret
- Channel Access Token

- Channel Access Token需先點選右手邊的「Issue」按鈕設定Token過期時效（若怕太快過期可設定24小時）後，才可取得

- 「Channel Secret, Channel Access Token」是讓Line官方能辨識Bot的重要資訊
- 需注意這些資訊請勿外流給其他人知道，否則他人將有機會偽造你的Bot回傳訊息給你的使用者


## 7.撰寫LINE Bot Node.js程式

## 參考資料
- 使用Node.js建置你的第一個LINE BOT : https://medium.com/pyradise/%E4%BD%BF%E7%94%A8node-js%E5%BB%BA%E7%BD%AE%E4%BD%A0%E7%9A%84%E7%AC%AC%E4%B8%80%E5%80%8Bline-bot-590b7ba7a28a
- How To Install Node.js on Ubuntu 16.04 : https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04
- How to install Node.js and npm on Ubuntu 18.04 : https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/
- 第 17 天：安裝 Node.js 及 NPM : https://ithelp.ithome.com.tw/articles/10194339
- LineBot+Python，輕鬆建立聊天機器人 : https://yaoandy107.github.io/line-bot-tutorial/
- Day27 關於LINE Bot 還有這些注意事項！(3) : https://ithelp.ithome.com.tw/articles/10206767


