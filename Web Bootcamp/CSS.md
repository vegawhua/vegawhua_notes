# Content
## Introduction
- [Inline CSS](#inline-css)
  * [Table](#table)
  * [Forms](#forms)
- [Internal CSS](#internal-css)
  * [border-style syntax](#border-style-syntax)
- [External CSS](#external-css)
- [Debug](#debug)
## Intermediate
CSS: Cascading Style Sheets 层叠样式表

# Introduction
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
### Pseudo class 伪类
添加到选择器的关键字，指定要选择的元素的特殊状态。例如，:hover 可被用于在用户将鼠标悬停在按钮上时改变按钮的颜色。
```
img:hover {
    background-color: white;
}
```

# Intermediate
## Favicons
Favicon是favorites icon的缩写，亦被称为website icon、page icon或urlicon。Favicon是与某个网站或网页相关联的图标。网站设计者可以多种方式创建这种图标，而目前也有很多网页浏览器支持此功能。

## HTML Divs
`div` - Special HTML element that allows to divide content up on the website so that we can structure each div separately.




