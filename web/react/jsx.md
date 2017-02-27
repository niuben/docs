JSX转换是通过`babel`工具进行的。
JSX的标签将转换为`React.createElement(type, config, children)`
* type: 标签名称;
* config: 属性配置；
* 子元素： 内容或者子element。

## 不能在JSX中使用`if-else`
`if-else`格式不能在JSX中出现。因为JSX只是转换成对象或者函数的语法糖，看下面基础例子

```
//jsx
<div id={if(true){'ms'}}>hello world</div>
```
转化成react element
```
react.createElement('div', {id: if(true){'ms'}}, "hello world");
```
如果使用`if-else`格式，上面代码格式是不正确的。

### 使用三元表达式
```
<div id={condition ? 'msg': null}>hello world</div>
```
转化成react element
```
react.createElement('div', {id: condition ? 'msg': null}, "hello world");
```
三元表达式有的时候有点捉襟见肘，可以在JSX之外使用`if-else`来决定使用哪个
```
  var id;
  if(condition) {
    id = msg;
  }
  return(
    <div id={id}>hello world</div>
  );
```
为了更多的内联，可以在jsx中定义"immediately-invoked"
```
return (
  <section>
    <h1>Color</h1>
    <h3>Name</h3>
    <p>{this.state.color || "white"}</p>
    <h3>Hex</h3>
    <p>
      {(() => {
        switch (this.state.color) {
          case "red":   return "#FF0000";
          case "green": return "#00FF00";
          case "blue":  return "#0000FF";
          default:      return "#FFFFFF";
        }
      })()}
    </p>
  </section>
);


```


## Self-Closing标签





## JSX扩展属性


## JSX注意事项
