# webpack2

## Tree-Sharking
可以将没有import的export代码删除。
### 实现
* lib/FlagDependencyUsagePlugin.js 实现将modules中使用过的exports，打包到module中；

## Hot Modules Replace 





## Coding Splitting Libraries

## Dependency Management

## Module Rules

## Configuration

### Watch And WatchOptions
监听文件是否变化，一旦文件变化进行重新编译。

#### watch 
_boolean_ 开启监听模式。

#### watchOptio 
object 自定义选项

_aggregateTimeout_: number 延迟编译的时间，可以避免频繁编译。单位是毫秒  
```aggregateTimeout: 300 //默认是300毫秒```

_ignored_: 忽略对一些文件夹的监听。因为监听大量的文件夹会消耗大量CPU内存，特别是像__node_modules__这样巨大的文件夹。  
```ignored: /node_modules/```
也可以使用_anymatch_格式。  
```ignored: "files/**/*.js```

_poll_: boolean/number 设置为true或者数字的话，将周期检查文件变化。单位是毫秒  
`poll: 1000 //每隔一秒钟检查一次` 

### target 
string webpack可以为多种环境进行编译。  

### Externals
为依赖模块不放在Bundle中提供一个方式。分别有：string，array，object，function

### 



 




