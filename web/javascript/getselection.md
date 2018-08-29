## getSelection 
这是全局API，用于返回一个选中对象。

```
    var selection = window.getSelection();    
```

### Range
用于选中的片段。

```
    var range = document.createRange(); //创建一个片段
    range.selectNode(document.querySelector("p"));  //设置片段选中的元素
    selection.addRange(range); //让选中对象增加一个判断;
```


[详细文档](http://help.dottoro.com/ljxaltpn.php)