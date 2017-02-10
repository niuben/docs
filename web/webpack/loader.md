#Loader
## html-loader
默认将模板里面的Img标签，改成require方式。

### 根路径

### attrs
可以指定需要解析哪些些属性，默认是img标签src属性
```html
<!-- demo.html -->
<link rel="stylesheet" type="text/css" href="./reset.css" />
<img src="./logo.png" />
```
```
<!--webpack config -->
module: {    
  loaders: [{
     test: /\.(png|css)$/,
     loader: 'file-loader?name=static/[hash].[name].[ext]'
   }]
}
// ...
```

```js
 require("html-loader?attrs[]=img:src&attr[]=link:href!./demo.html");
 // => <link rel="stylesheet" type="text/css" href="static/afc47bf1a6696c427189aa6fc7cf3ee8.reset.css" />
 // => <img src="static/59294d87d6f98581b837246820795d81.logo.png" />
```
