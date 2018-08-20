# express
- 初始化專案  
    ```bash
    express -f 專案名稱
    ```
- install package  
    ```bash
    #兩者擇一執行
    yarn install
    npm install
    ```  
    初始後, 使用`npm install`或`yarn install`安裝 package.json 內所指定的套件, 安裝後會產生 node_modules 資料夾  
- routes/index.js 加入 /test 路徑, 並傳送文字  
    `router.get` 代表建立一個路由並使用 HTTP request methods 中的 get 形式.  
    ```javascript
    router.get('子路徑', function(接收資料, 回傳資料, next) {
        res.send('顯示的文字')
    })
    ```
- 執行  
    使用 `node ./bin/www` 或 `npm start` 來啟動專案(localhost:3000)  
    `npm start` 是在 package.json 檔案裡的 script 所設定的快捷鍵
    ```bash
    #兩者擇一執行
    node ./bin/www
    npm start
    ```
