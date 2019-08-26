><br/>
>
>HTML       ---- 內容
>CSS        ---- 畫面的呈現
>JavaScript ---- 動作
>Developer Tools F12按下去! (safari 要開啟開發者模式)
><br/>



#HTML
## Element
     ┌───── tag的開頭
     │   ┌───── attribute                 ┌───── attribute
    <a href="https://www.google.com.tw" target="_blank"> 
        這是一個超連結會連到google去            ───────── content
    </a>
      └─tag的結尾
由tag和content組成

<a href="https://www.google.com.tw" target="_blank"> Goooogle </a>



-------



## 架構
    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8">
        <title>My test page</title>
    </head>
    <body>
        <img src="https://cdn.imgbin.com/0/24/2/imgbin-shaun-the-sheep-puzzle-putt-film-stop-motion-television-show-sheep-6ks2TVGD89HHMFfgenWDe4sFE.jpg" alt="My test image">
    </body>
    </html>

* **&lt;!DOCTYPE html&gt;**
    文件類型: 告訴瀏覽器要使用哪個版本進行編寫
* **&lt;html&gt;&lt;/html&gt;**
    根目錄
* **&lt;head&gt;&lt;/head&gt;**
    重要資訊，但不會顯示於網頁瀏覽者眼前的
    title, 各種meta(og-title, og-image, ...), css
* **&lt;title&gt;&lt;/title&gt;**
    網頁標題
* **&lt;meta charset="utf-8"&gt;**
    指定文件使用utf-8這種字元編碼
* **&lt;body&gt;&lt;/body&gt;**
    顯示於網頁瀏覽者眼前的內容



-------



## 常用特殊符號
HTML 原始碼 |顯示 結果
:---------:|:------:
&amp;lt;  | &lt;
&amp;gt;  | &gt;
&amp;amp; | &amp;
&amp;nbsp;| &nbsp;
...還有更多



--------



## 常用tag

        <span>我是span</span><span>我是span</span>
    
> <span>我是span</span><span>我是span</span>

        <div>我是div</div><div>我是div</div>

> <div>我是div</div><div>我是div</div>

        我有br<br/>我有br<br/>


> 我有br<br/>我有br<br/>

        <p>我是p</p><p>我是p</p>

> <p>我是p</p><p>我是p</p>


        <h1>我是h1</h1>
        <h2>我是h2</h2>
        <h3>我是h3</h3>
        <h4>我是h4</h4>
        <h5>我是h5</h5>
        <h6>我是h6</h6>

><br/>
><h1>我是h1</h1>
><h2>我是h2</h2>
><h3>我是h3</h3>
><h4>我是h4</h4>
><h5>我是h5</h5>
><h6>我是h6</h6>
><br/>


        <iframe src="https://www.family.com.tw/Marketing/index.aspx"></iframe>
><br/>  
><iframe src="https://www.family.com.tw/Marketing/index.aspx"></iframe>
><br/>


        // rowspan: 佔據幾個直排, colsapn: 佔據幾個橫排
        <table>
            <thead>
                <tr>
                    <td>head1</td>
                    <td>head2</td>
                    <td>head3</td>
                    <td>head4</td>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td rowspan="2">body1</td>
                    <td>body2</td>
                    <td colspan="2">body3</td>
                </tr>
                <tr>
                    <td>body5</td>
                    <td>body6</td>
                    <td>body7</td>
                </tr>
            </tbody>
        </table>

><br/>
><table>
>    <thead>
>        <tr>
>            <td>head1</td>
>            <td>head2</td>
>            <td>head3</td>
>            <td>head4</td>
>        </tr>
>    </thead>
>    <tbody>
>        <tr>
>            <td rowspan="2">body1</td>
>            <td>body2</td>
>            <td colspan="2">body3</td>
>        </tr>
>        <tr>
>            <td>body5</td>
>            <td>body6</td>
>            <td>body7</td>
>        </tr>
>    </tbody>
></table>
><br/>



-------



## 表單

* method
    * GET: 傳送的資料會在網址後方使用querystring的方式被送出
    * POST: 資料會被放在訊息主體(message body)中發送, 但是header中會有比GET夾帶多一些資訊(Content Length, Content-Type...)所以封包會比較大一點

<br/>

        <form action="https://www.w3schools.com/action_page.php" target="_blank">
            <div>
                <label>姓名：</label><input type="text" name="userName">
            </div>
            <div>
                <label>性別：</label>
                <input type="radio" value="male" name="gender" id="gender_1"><label for="gender_1">男</label>
                <input type="radio" value="female" name="gender" id="gender_2"><label for="gender_2">女</label>
            </div>
            <div>
                <label>喜歡的食物類型：</label>
                <input type="checkbox" value="1" name="fType" id="fType_1"><label for="fType_1">中式</label>
                <input type="checkbox" value="2" name="fType" id="fType_2"><label for="fType_2">西式</label>
                <input type="checkbox" value="3" name="fType" id="fType_3"><label for="fType_3">日式</label>
                <input type="checkbox" value="4" name="fType" id="fType_4"><label for="fType_4">韓式</label>
            </div>
            <div>
                <label>居住地區：</label>
                <select name="area">
                    <option selected disabled>請選擇</option>
                    <option value="台北市">台北市</option>
                    <option value="新北市">新北市</option>
                    <option value="桃園市">桃園市</option>
                    <option disabled>...</option>
                </select>
            </div>
            <div>
                <input type="submit" >
                <input type="reset">
            </div>
        </form>

><br/>
><form action="https://www.w3schools.com/action_page.php" target="_blank">
>    <div>
>        <label>姓名：</label><input type="text" name="userName">
>    </div>
>    <div>
>        <label>性別：</label>
>        <input type="radio" value="male" name="gender" id="gender_1"><label for="gender_1">男</label>
>        <input type="radio" value="female" name="gender" id="gender_2"><label for="gender_2">女</label>
>    </div>
>    <div>
>        <label>喜歡的食物類型：</label>
>        <input type="checkbox" value="1" name="fType" id="fType_1"><label for="fType_1">中式</label>
>        <input type="checkbox" value="2" name="fType" id="fType_2"><label for="fType_2">西式</label>
>        <input type="checkbox" value="3" name="fType" id="fType_3"><label for="fType_3">日式</label>
>        <input type="checkbox" value="4" name="fType" id="fType_4"><label for="fType_4">韓式</label>
>    </div>
>    <div>
>        <label>居住地區：</label>
>        <select name="area">
>            <option selected disabled>請選擇</option>
>            <option value="台北市">台北市</option>
>            <option value="新北市">新北市</option>
>            <option value="桃園市">桃園市</option>
>            <option disabled>...</option>
>        </select>
>    </div>
>    <div>
>        <input type="submit" >
>        <input type="reset">
>    </div>
></form>
><br/>



-----



#CSS

## 基本顯示方式

* inline: 寬度會根據內容做改變, 無法透過css調整其寬度跟高度 
* block: 寬度會佔據一整行, 可以透過css調整寬高
* inline-block: 寬度會根據內容做改變, 可以透過css調整寬高


### [css selector](https://www.w3schools.com/cssref/css_selectors.asp)
    
    <style>
        .color-red{
            /* class="color-red" */
            color: red;
        }

        #green{
            /* id="green" */
            color: green;
        }

        div{
            /* <div></div> */
            color: blue;
        }

        .parent .child{
            background: black;
        }

        .parent.mother{
            background: pink;
        }
    </style>

### [css specificity](https://www.w3schools.com/css/css_specificity.asp)
        
        !important 是規格外, 少用
        style > id > class > element

        inline style: 1000
        id: 100
        class: 10
        element: 1



-----



#JavaScript

## 如何使用

        // 方法1 在head或body中放置script元素
        <script>
            alert('Hello World!');
        </script>

        // 方法2 載入外步的js
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>

        // 方法3 在element上的on開頭屬性中撰寫
        <button onclick="alert('我在測試!')">測試</button>

## 資料型別
* Null
* Undefined
* Number
    * （在 -(253 -1) and 253 -1 之間的數字）
    * 能代表浮點數
    * Infinity, -Infinity 代表正負數的無窮大
    * NaN 不是數字
* Boolean
* String
* Object

##### 可使用 typeof 來取得變數的型別
    typeof 123 // "number"

## 變數宣告
    
    /* 我是註解 */
    // 我也是註解

    // 變數名稱大多使用駝峰式命名: OnClick, onClick
    // 不使用var會被當作全域變數進行宣告
    dontDoIt = '不要這樣做';

    // 推薦使用的變數宣告
    var firstString = 'Hello World!';

    // 物件實字
    var userData = {
        name: 'John',
        id: 1
    };

    // 不推薦
    var userData = new Object();
    userData.name = 'John';
    userData.id = 1;

    // 取得物件屬性的value
    userData.name; // "John"
    userData['id']; // "1"

    // 陣列實字
    var numberList = [1,2,3,4,5,6,7];

    // 不推薦
    var numberList = new Array(1,2,3,4,5,6,7); 
    new Array(3); // [undefined, undefined, undefined]

## 運算子
[MDN這裡都有](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Guide/Expressions_and_Operators)

    // 嚴格等於 ===
    // 嚴格不等於 !==
    var numA = 123,
        StrA = '123';
    numA == StrA; // true
    numA === StrA; // false

## 迴圈
[MDN這裡都有](https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Reference/Statements)

    // for...in
    var ary = [1,2,3,4,5,6];
    for (var index in ary) {
        console.log(index); // 0,1,2,3,4,5
    }

    var user = { name: 'John', id: 1};
    for (var prop in user) {
        console.log(prop); // name, id
    }

## 動態網頁、靜態網頁的差別

* 動態網頁
    * 在使用者操作後畫面會進行回饋(改變內容, 樣式)
    * 資料由後端提供, 會根據取得的資料結果呈現不同的結果
* 靜態網頁
    * 純文字資料無任何與使用者的互動
    * 資料固定不變

## DOM
[W3CSCHOOOLS這裡都有](https://www.w3schools.com/js/js_htmldom.asp)

* 提供給開發者對文件進行動態操作(新增、更新、刪除)的介面
* Core DOM(XML,HTML皆可使用的操作), XML DOM, HTML DOM
* 透過Javascript來操作HTML DOM改變網頁的內容

        <div id="testId">我的id是testId</div>

        <script>
            var testEle = document.getElementById('testId');
            console.log(testEle);
            testEle.style.color = 'red';
        </script>


## 非同步 Asynchronous

    // 超。簡易說明
    // 一直到被觸發才會去執行 在倒數的過程中不會阻塞後續程式的執行
    setTimeout(function () {
        console.log('YOOOOOOOO!');
    }, 3000);
    console.log('wait!');

    // wait!
    // Yooooooo!

## Json
* [輕量級的資料交換語言](https://zh.wikipedia.org/wiki/JSON)
* number: 

        123
* string:

         "123456789"
* boolean: 

        true, false
* object: 

        { "id": 1, "name": "John"}
* array: 

        [
            { "id": 1, "name": "John"}, 
            { "id": 2, "name": "Marrry"}
        ]

## Ajax

        var httpRequest = new XMLHttpRequest();
        // 告訴瀏覽器伺服器回傳的資料要用什麼type處理 
        httpRequest.overrideMimeType("application/json");
        
        // 註冊一個onreadystatechange事件
        // 當readystate改變時觸發對應的函數
        httpRequest.onreadystatechange = function () {
            try {
                if (httpRequest.readyState === XMLHttpRequest.DONE) {
                    // 伺服器回傳的status code
                    if (httpRequest.status === 200) {
                        // 將接收到的json文字轉為 js Object使用
                        var res = JSON.parse(httpRequest.responseText);
                        alert('res.name: ' + res.name);
                    } else {
                        alert('There was a problem with the request.');
                    }
                }
            } catch(e) {
                alert('Caught Exception: ' + e.description);
            }
        };

        httpRequest.open('GET', './data.json', true);
        httpRequest.send();
    
<button onclick="activeAjax()">發送</button>
<script>
    function activeAjax() {
        var httpRequest = new XMLHttpRequest();
        httpRequest.overrideMimeType("application/json");
        httpRequest.onreadystatechange = function () {
            try {
                if (httpRequest.readyState === XMLHttpRequest.DONE) {
                    if (httpRequest.status === 200) {
                        var res = JSON.parse(httpRequest.responseText);
                        alert('res.name: ' + res.name);
                    } else {
                        alert('There was a problem with the request.');
                    }
                }
            } catch(e) {
                alert('Caught Exception: ' + e.description);
            }
        };

        httpRequest.open('GET', './data.json', true);
        httpRequest.send();
    }
</script>