# Content
- [HTML Tag](#html-tag)
  * [Table](#table)
  * [HTML - Personal Site](#html---personal-site)
  * [Forms](#forms)
- [Dict](#dict)
- [Recommend Tool](#recommend-tool)

## HTML Tag  
\<HTML element HTML attribute>  
  
| Tag name | Function | Comment | Example |
| -------- | -------- | ------- | ------- |
| `<h1></h1>...<h6></h6>` | | Heading Format | `<h1>title</h1>` |
| `<br>` | Insert space between items | Self-closing | |
| `<hr>` | Add horizontal lines | Self-closing | `<hr size = "3" noshade>` |
| `<center></center>` | | |
| l16开始`<p></p>` | Paragraph tag | | |
| `<em></em>` | Emphasize the content and Italisized it, **Prefer** | | |
| `<i></i>` | Style: Only italisized the content | No emphasis, no info | |
| `<strong></strong>` | Text has strong importance, **Prefer** | Bold and confer info | |
| `<b></b>` | Style: make the content bold | No meaning | |
| `<ul></ul>` | An Un-ordered List | | `<ul> <li></li> </ul>`|
| `<ol></ol>` | An Ordered List | |`<ol type = "i"> <li></li> </ul>` |
| `<img src = "">` | Add image to the page | Self-closing | `<img src="vega.png"> `|
| `<a href="link destination"> link text</a>` | **Anchor tag** Add hyperlink | | `<a href="https://">hi</a>` |
| `<input type="text">` | Form tag, with `<label></label>` | Self-closing | |
| | | | |
| Special | | | |
| \<!-- xxx --> | Make comment | | |

### Table
Attributes have been deprecated  
```html
<!-- <table cellspacing = "5"> -->
<table>  
  <!-- <thead align="left"> -->
  <thead>
    <!-- table row -->
    <tr>
      <!-- table head data -->
      <th>...</th>    
      <th>...</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <!-- table data -->
      <td>...</td>    
      <td>...</td>
    </tr>
  </tbody>
</table>      
```

### Forms
**Basic**
```html
<!-- action: Jump to this page after pressing the button -->
<form class="" action="index.html" method="post">
 <label for="">Your name: </label>
 <input type="text" name="" value="">
 <input type="color" name="" value="">
 <label for="">Password:</label>
 <input type="password" name="" value="">
 <label for="">Text your message:</label>
 <textarea name="name" rows="10" cols="30"></textarea>
 <input type="submit" name="" value="Submit">
</form>
```
**Output:**  
![form_example](https://user-images.githubusercontent.com/97777280/149737429-4e1bddfb-4939-4937-9813-788be257a8b2.png)

**Advanced**
```html
<form action="mailto:vega.huangx@gmail.com" method="post" enctype="text/plain">
 <label for="">Your name: </label>
 <input type="text" name="Yourname" value="">
 <label for="">Your Email:</label>
 <input type="email" name="Youremail" value="">
 <label for="">Text your message:</label>
 <textarea name="Yourmessage" rows="10" cols="30"></textarea>
 <input type="submit" name="" value="Submit">
</form>
```
**Output:**  
![emailto_example](https://user-images.githubusercontent.com/97777280/149739387-ea8cb7c5-d2a5-4a88-a4c9-2faf0ee1b7f5.png)



### HTML - Personal Site
```html
<!-- Emmet: quick coding - input 'html' and press enter -->

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>

  </body>
</html>

```


## Dict
- \<tag name> - angular brackets < >

## Recommend Tool
- [devdocs](https://devdocs.io)
- Hosting sites
  - Paid
    - [GoDaddy](https://www.godaddy.com/)
    - [Bluehost](https://www.bluehost.com/)
  - Free: [Github](https://github.com/) - Lesson28
