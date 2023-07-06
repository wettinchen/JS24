## JavaScript Chapter 24
It is my coding practice with the TUTORIAL of Dave Gray. 

## Source
### Dave Gray 的 JavaScript 課程
https://youtube.com/playlist?list=PL0Zuz27SZ-6Oi6xNtL_fwCrwpuqylMsgT

### Dave Gray 的 YouTube 頻道
https://www.youtube.com/@DaveGrayTeachesCode

## JavaScript Chapter 24
   Quick Concept outline
   中文摘要說明與重點提問

###  1. Intro 
        教學影片開頭和介紹

###  2. ES6 Module Basics
        從一個資料夾，匯出不同的程式部分，匯入到另一個資料夾，通常是函數 function 或 class

###  3. JS Modules are only supported on servers
        說明 JavaScript 模組只支援伺服器，不支援其他路徑
    
###  4. Use the Live Server extension in VS Code
        點擊 Extensions 搜尋 Live Server

###  5. The script tag with type="module"
        html 匯入的 JavaScript 標籤為 type="module"

###  6. No defer needed
        第一點自動採用 defer關鍵字

###  7. Strict mode by default
        第二點預設採用 strict 模式: 如同在 JavaScript 輸入 use strict

###  8. Create a Javascript Module
        創設一個 JavaScript 模組 guitars24QCo08.js

###  9. Export default
        設定匯出的預設值為 playGuitar 函數

### 10. Export { firstItem, secondItem }
        匯出其他函數 shredding, plucking

### 11. Export inline
        在同一行匯出export第一行、第二行和第三行，第一行為 default預設值

### 12. Import the default export
        從 guitars24QCo12.js 匯入 playGuitar 函數 至 main24QCo12.js

### 13. Import { firstItem, secondItem }
        從 guitars24QCo13.js 匯入 shredding 函數和 plucking 函數 至 main24QCo13.js

### 14. Rename imports
        使用 Import { firstItem as firstRename, secondItem as secondRename }，將 shredding 重新命名為 shred，plucking 重新命名為 fingerpicking

### 15. Import the full namespace
        Import * as Name，無法重新命名各別函數
        (1)從 guitars24QCo15.js 匯入使用 Import * as Guitar，
        重新命名為 Guitar，修改匯出格式；但是會回傳 Uncaught TypeError: playGuitar is not a function。
        (2)修正錯誤，第一個匯出的函數為預設值，使用 Guitar.default 回傳函數
        (3)移除 playGuitar() 不作為預設值，修改函數回傳 playGuitar函數

### 16. JavaScript Class export and import example
        新增 user24QCo16.js，匯出預設值，宣告 class 名稱為 User；
        在物件宣告 constructor建構子，參數為 email 和 name；
        使用 this 關鍵字宣告 id 回傳 email，name 回傳 name。宣告 greeting 函數作為方法，回傳 Hi, my name is 名字。

        從 user24QCo16.js 匯入 User，宣告 me 為 new User函數，信箱參數為 email@email.com，名字參數為 Dave，並回傳 User 的 object 和 Hi, my name is Dave。

### 17. Current browser support for modules
        https://caniuse.com/?search=module