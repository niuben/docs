# react 

## 代码结构

### react和react-dom
`为什么会分开`

## 组件

## 自定义标签

## 事件系统
### 合成事件
定义的事件都会成为合成事件的实例，合成事件包含原生事件（相同的API），包括`stopPropagation()`和`preventDafult()`，并且跨浏览器。
因为某些原因想知道浏览器内部事件，可以简单使用`nativeEvent`属性得到它们。每个合成事件都包含下面属性
```
    booleans bubbles
    booleans cancelable
    DOMEventTarget currentTarget
    booleans dafaultPrevented
    Number eventPharse
    booleans isTrusted
    DOMEvent nativeEvent
    void  preventDafault
    booleans isDafaultPrevented()
    void  stopPropagation()
    booleans isPropagationStopped()
    DOMEventTarget target
    Number timeStamp
    String  type 

```
### Event Pooling

### 支持事件列表

#### 剪切板事件
事件列表
* onCopy
* onCut
* onPast

属性值：`DOMDataTransfer clipboardData`

#### Composition事件
事件列表
* onCompositionEnd
* onCompositionStart
* onCompositionUpdate
属性值：`strig data`


#### 键盘事件
事件列表
* onKeyDown
* onKeyUp
* onKeyPress

属性值：
 

#### 通过class进行事件绑定



## 虚拟DOM

## JSX实现

## 状态和属性

## 生命周期

## API

### Top-Tevel 

#### React.Componet

#### React.createClass

#### React.createElement

#### React.cloneElement

#### React.createFactory

#### React.isValiElement

#### React.DOM

#### React.propType

#### React.Children

_React.Children.forEach_


_React.Children.count_

_React.Children.only_

_React.Children.toArray_

#### ReactDOM.render

#### ReactDOM.unmoutComponentAtNode

#### ReactDOM.findDOMNode

#### ReactDOMServer.renderToString

#### ReactDOMServer.renderToStaticMarkup

### 组件 API

#### setState
`js
setState(
    function | object,
    [function callback]
)
`
> function(state, props) 两个参数：当前状态和属性

#### replaceState
`js
replace(
    object,
    [function callback]
)
`

#### fouceUpate 


#### isMounted
`js
booealn isMounted()
`

### 组件规格和生命周期

#### render
` ReactElement render() `

#### getInitialState
` Objeact getInitialState() `

#### getDefaultProps
` Objectt getDefalutProps() `

#### propTypes
` Object propTypes `
验证chuangding

#### mixins
` array mixins `  
多个组件之间共用一些方法

#### statics
` object static `
在static对象下定义方法，可以在class下使用这个方法
`
    var MyComponent = React.createClass({
        statics: {
            customMethod: function(){
                console.log("static")
            }
        }
    });

    MyComponent.customMethod() //static
`
#### displayName 
用于代码调试，类将自动设置该值。 `test`

#### [Mounting] componentWillMount

#### [Mounting] componentDidMount

#### [Updating] componentWillReceiveProps

#### [Updating] shouldComponentUpdate

#### [Updating] componentWillUpdate

#### [Updating] componentDidUpdate

#### [Unmounting] componentWillUnmount

## dangerouslysetinnerhtml
不让react自动转移特殊字符；

 




