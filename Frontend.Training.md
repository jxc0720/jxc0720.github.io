# 前端? 後端? 全端??

---

# 前端
## 作業流程
  1. 設計師提供網站的設計圖和切好的素材圖片
  2. 進行切版
  3. 資料串接

---

## 響應式? RWD?
  * 使用 css 中的 [media queries](https://www.w3schools.com/css/css3_mediaqueries_ex.asp) 來針對不同裝置寬度進行調整
  * js 也有 [media queries](https://www.w3schools.com/howto/howto_js_media_queries.asp)

## 專案常用到的
* [html, css, js](https://www.w3schools.com/)
* [jQuery](https://api.jquery.com/)

## [Ajax](https://www.w3schools.com/js/js_ajax_intro.asp)
  * 非同步
  * XMLHttpRequest
  * rquest
  * response

## 資料交換格式
* [JSON](https://www.w3schools.com/js/js_json_intro.asp)

      {
        "name": "John",
        "list": ["a", "b", "c"],
        "data": {
          "birthday": "19870807"
        }
      }
  
  * int, string, boolean, array, object, null
  * js 可使用 JSON.parse 轉換為 js object 來使用
<br/>

* [XML](https://www.w3schools.com/xml/)

      <?xml version="1.0" encoding="UTF-8"?>
      <note>
        <to>Tove</to>
        <from>Jani</from>
        <heading>Reminder</heading>
        <body>Don't forget me this weekend!</body>
      </note>
  * string
  * js 可透過 [DOMParser](https://www.w3schools.com/xml/xml_dom.asp) 轉換為 dom物件 來取得結點的內容

## 你可能需要知道的
* [es5](https://www.w3schools.com/js/js_es5.asp), [es6](https://www.w3schools.com/js/js_es6.asp)
* [node js](https://nodejs.org/en/)
* [npm](https://www.npmjs.com/)
* [babel](https://babeljs.io/)
* [react](https://zh-hant.reactjs.org/)