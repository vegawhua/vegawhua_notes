# Concept
**CSS: Cascading Style Sheets 层叠样式表**
## Inline CSS
内联: cannot implement to all tags in the webpage at once, need to be revised one by one
```html
<body style="background-color:cornsilk;">
```

## Internal CSS
内部: cannot be consistent across the website, cannot carry over to all other web pages on the website.  
Solution:  
A single location where when the CSS styles have been changed in that one location, then everything gets reflected across our website in all of the pages. 
```html
<head>
  <meta charset="utf-8">
  <title>❤️Vega's Personal Site</title>
  
  <style>
    body{
      background-color:cornsilk;
    }
    hr{
      border-style:none;
      border-top:7px dotted grey;
      width:4%;
    }
  </style>
</head>
```

### border-style syntax
- The border-style property may be specified using **one**, **two**, **three**, or **four** values.
  - When **one** value is specified, it applies the same style to all four sides.
  - When **two** values are specified, the first style applies to the top and bottom, the second to the left and right.
  - When **three** values are specified, the first style applies to the top, the second to the left and right, the third to the bottom.
  - When **four** values are specified, the styles apply to the top, right, bottom, and left in that order (clockwise).

## External CSS
make pages consistent
`<link rel="stylessheet" href="css/style.css">`
<img width="810" alt="image" src="https://user-images.githubusercontent.com/97777280/154622209-911f7e08-cbf5-49f7-8322-ead21b6d5298.png">

## Debug
style priority:  
1. inline CSS
2. internal CSS
3. external CSS

## CSS Syntax
`selector {property:value;}`
Keep all of rules in alphabetical order

## CSS Selectors
`selector {property:value;}` - Tag Selectors  
`class=""` - Class Selectors - differentiate all of different HTML elements, making specific styling

## Classes vs. Ids
Identify HTML elements
- `id` is unique inside a single page. 
  - identify elements where there is only a single one of them on a particular page.
  - it's not suggested to be used in CSS styling.
- `class` can be the same, and each element can have several classes.
  - group related elements that are all going to behave or have a similar style.
### Pseudo class 
伪类：添加到选择器的关键字，指定要选择的元素的特殊状态。例如，:hover 可被用于在用户将鼠标悬停在按钮上时改变按钮的颜色。
```
img:hover {
    background-color: white;
}
```

# Intermediate
## Favicons
Favicon是favorites icon的缩写，亦被称为website icon、page icon或urlicon。Favicon是与某个网站或网页相关联的图标。网站设计者可以多种方式创建这种图标，而目前也有很多网页浏览器支持此功能。

## HTML Divs
`div` - A content division element that allows to divide content up on the website so that we can structure each div separately.
- Don't do anything unless using CSS

## Box Model
- height & width: static value or percentage
- border: `{border-width:0px;}` / `{border-width:0px 10px 20px 10px;}`
- padding: `{padding：20px;}` - 内容离box边缘的距离
- margin: `{margin:20px;}` - box离viewspot的距离

## CSS Display Property
CSS显示属性
CSS`display` Swift between Block and Inline
- Block: Take a whole width of the screen on a web page by default. 可以调整高度宽度
  - Paragraphs `<p>`
  - Headers `<h1>` - `<h6>`
  - Divisions `<div>`
  - Lists and list items `<ol>` `<ul>` `<li>`
  - Forms `<form>`
- Inline - 可以同一行，但是高度宽度无法调整，是根据内容固定的
  - Spans `span`: Select one part of the text. 
  - Images `<img>`
  - Anchors `<a>`
- Inline-Block
- None
  - `{display:none}`:消失，不保留位置
  - `{visiblity:hidden}`:消失，保留位置

## Fonts
Lesson 97  
Readability & Legibility  
Prefer 2 fonts in one design  
Serif typeface - 字母下面有脚脚
- Old Style
- Transitional
- Modern
- **Slab-Serif**
Sans-serif 

## CSS Static and Relative Positioning
Rules:  
1. Content is Everything
2. Order Comes From Code
3. Children Sit On Parents
**Postion**  
- Static(Default)
- Relative
 - 和margin不同的是，relative会保留其他element不变化（可能产生覆盖），margin会让其他element跟着一起动
 ```
 img {
  position: relative;
  right: 30px;
 }
 ```
- Absolute: 是element相对于其parent div的位置，常指整个页面
> absolute是绝对定位；而relative是相对定位； 解释： 绝对定位就是相对于父元素的定位，不受父元素内其他子元素的影响；而相对定位是相对于同级元素的定位，也就是上一个同级元素!
- Fixd：导航栏就是这样的，翻页不动项

**Coordinates**  
- Top
- Bottom
- Left
- Right

## Center the elements
`{text-align: center}` - be set inside the parent container.
`{margin: 0 auto 0 auto}` - auto代表自动纵向横向的居中，用在有width限制的element上

## Font Styling
内置字体：
1. Serif - default: Times
2. Sans-serif - default: Arial  `{font-family: verdana, sans-serif;}`
3. Monospace - 常用于展示代码，易读性强  
  
如果想确保未安装首选字体的设备可以正常浏览，可以由specific --> less specific顺序依次指定展示的字体  
```
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif
}
```  
Font Embedding: 如果希望所有设备都浏览到指定的字体 have the same viewing experience  

-----2.19-----
## CSS Sizing
### font-size
|单位|分类|特点|换算|
|------|------|------|------|
|em|Dynamic|1em代表一个大写M的size, **value在parent body的size上累加**| 1em |
|px|Static|parent变它不变| 16px |
|%|Dynamic|**value在parent body的size上累加**| 100% |
|rem|Dynamic|CSS3，ignore all of the parent settings for the font size and set it to this relative to the root.忽略字体大小的所有父设置，并将其设置为此相对于根。| 1rem |
> Tip: **Using `rem`** instead of `em` or `%`

### color
修改文本字体颜色

### font-weight
字体的粗细 - normal or bold  
e.g. `{font-weight: normal;}`

### line-height
设置多行元素的空间量，如多行文本的间距
e.g. `{line-height: 2;}`

## CSS Float and Clear
- float: use for **wrapping** not for **positioning** - 用position: relative / absolute或者margin / padding
  - 指定一个元素应沿其容器的左侧或右侧放置，允许文本和内联元素环绕它。  
  - value: none / left / right  
- clear (anti-float)
  - 指定一个元素是否必须移动(清除浮动后)到在它之前的浮动元素下面。  
  - value: none / left / right / both
>网页虽然差不多设置好了，但是它还不是responsive反应灵敏的 --> 引出Bootstrap -->让website适用于all screen sizes and all dimensions.

