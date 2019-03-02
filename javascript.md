## javascript 


### 第1章: 基本概念
__1.1 语法__ 

区别大小写敏感。
标识符是指变量名、类名和函数名等。标识符命名规则如下  

* 首字母必须为下划线(_)、字母或者美元符;  
* 非首字母可以为下划线、字母、美元符和数字;  

使用”use static"启动严格模式。  
每条语句用“;"结束。

__1.2 变量__  
变量需要满足标识符命名规则。变量分为局部变量和全局变量;

__1.3操作符__
* 四则运算符: `+ - * / `
* 位操作符： `~ & | ^ << >> >>>`
* 布尔操作符：`！&& ||`
* 判断操作符：`> >= < <= == ===`
* 赋值操作符：`=`
* 条件操作符：`？:`

__1.4数据类型__
通过__typeof__操作符可以知道变量的数据类型，javascript有下面6种数据类型

* Undefined: 未定义
* Null: 空对象
* Object: 对象
* Number: 数字类型
* Boolean: 布尔类型 
* String: 字符串类型

u


__对象__
`Object`是`javascript`的内置对象，命名一个对象实际上是`new Object`一个实例。

```
    var obj = {a: 1};
    obj.constructor == Object; // true
    obj instanceOf Object; // true
```
* constructor：指向实例的构造函数;
* isPrototypeOf: 是否是它的原型;
* propertyIsEnumerable: 属性是否可枚举;

`__proto__`用于实例对象指向构造函数的原型链

```
    var obj = {a: 1};
    obj.__proto__ == Objeact.prototype; // true
```

__作用域__
作用域可以知道当前可访问的变量和函数；
作用域链是当前位置到`window`环境之间所有可访问变量和函数的集合。会从作用域链的顶端开始往下一个一个查找，直到Windows环境为止。


__函数__
闭包是指可以访问另一个函数里的变量或者函数; 闭包的本质是作用域链


### 事件

__移动端__  

touch事件:
* ontouchstart 
* ontouchmove
* ontouchend

touch和mouse事件区别:
* touch事件没有hover态;
* touch事件有多个接触点，而mouse事件则只有一个;

touch事件对象:
* touchevent
* touchlist
* touch

