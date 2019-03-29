## Node手册


#### 在vscode中调试node代码

* 打开vscodet调试;
* 点击配置icon，打开配置文件;
* 在配置文件中加入下面配置项:
```
    {
        "type": "node",
        "request": "launch",        
        "program": "${file}"
    }

```
* 将program字段填入需要调试的js文件地址;
* 点击开始调试;
