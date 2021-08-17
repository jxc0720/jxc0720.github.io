# 開始前

><br/>
>
>HTML       ---- 內容
>CSS        ---- 畫面的呈現
>JavaScript ---- 動作
>Developer Tools F12按下去! (safari 要開啟開發者模式)
><br/>

## 注意事項
* 瀏覽器的支援程度

## 公司內專案較常使用的瀏覽器
* IE11 (文件模式5)
* IE11
* Chrome
* safari (iOS)
* Chrome (Android)

----

#CSS

### [Specificity](https://www.w3schools.com/css/css_specificity.asp)
        
      style > id > class > element

      inline style: 1000
      id: 100
      class: 10
      element: 1

      !important 只能被 !important 覆蓋, 盡量少用

### [Selector](https://www.w3schools.com/cssref/css_selectors.asp)
    
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

        tr:nth-child(even) {
            background-color: blue;
            color: white;
        }
    </style>

## [Properties](https://developer.mozilla.org/zh-TW/docs/Web/CSS/CSS_Properties_Reference)

      /* 文字 */
      color: white;
      font-size: 16px;
      font-weight: normal;

      /* 邊框 */
      border: 1px solid black;
      border-radius: 8px;

      /* 背景 */
      background-color: gray;

      /* 距離 */
      line-height: 1.5;
      letter-space: 10px;
      padding: 1px 2px 3px 0px;
      margin: 0px auto;


## 基本顯示方式

* inline: 寬度會根據內容做改變, 無法透過css調整其寬度跟高度 
* block: 寬度會佔據一整行, 可以透過css調整寬高
* inline-block: 寬度會根據內容做改變, 可以透過css調整寬高

## 跳脫基本排版

* float
  * left
  * right
* position
  * relative
  * absolute
  * fixed

-----
