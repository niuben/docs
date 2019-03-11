## HTML
超文本标记语言（英语：HyperText Markup Language，简称：HTML）是一种用于创建网页的标准标记语言。

### HTML结构
一个完整网页会包含下面内容
1. 文档类型声明
2. html、head、title、body标签

```HTML
<!DOCTYPE html>
<html>
  <head>
    <title>This is a title</title>
  </head>
  <body>
    <p>Hello world!</p>
  </body>
</html>
```

### 文档类型声明
文档类型声明的初衷是通过基于文档类型定义（DTD）的SGML工具来解析并验证HTML文档。
DTD（Document Type Definition）是一个或多个XML模板。它定义XML元素、元素属性、元素排列方式和元素包内容。
浏览器根据不同文档类型会有不同解析模式，常见模式有下面两种
* 通用模式                                          ？
* 严格模式                                          ？

### 标签语义化
语义化是指通过文字表达功能。比如下面这段标签
```
    <p>hello <strong>world</strong>!</p>
```
通过标签名称就能理解`<strong>`是加粗的意思。  
开发的过程中尽量使用具有语义化的标签，这样可以大大提高标签语言的阅读效率;


### 标签类型
标签一般分为闭合标签和非闭合标签;   
闭合标签：有一个单独结束标签；比如`<body></body>`  
非闭合标签：没有单独结束标签；比如`<img />`  

闭合标签可以再嵌套其他的标签; 非闭合标签则无法再嵌套其他标签;


### 块状和行内标签
块状标签是指标签占据页面一整行；  
行内标签是指标签不占据页面一整行，后面元素也可以在这行显示;  
浏览器默认有些标签是块状标签、有些标签是行内标签;   

常见块状标签：
* div
* p
* h1~h6
* ul、li
* dt、dl、dh ?
* body
* form
* table
* code
* iframe

常见行内标签：
* span
* font
* strong
* bold
* i
* th、td








