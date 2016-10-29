[TOC]
#创建文件夹 ```app\Libs```  
修改composer.json
```
"autoload": {
    "classmap": [
        ...
        "app/Libs"
    ],
},
```
运行命令
```
 composer dumpauto
```
> 注意观察\vendor\composer\autoload_classmap.php

#在```Controller```里使用
##第一种方法
```
use ComoTool;
...
ComoTool::Filesize(111);
```
##第二种方法
```
\ComoTool::Filesize(111);
```
#在```view```里使用
```
{{ComoTool::Filesize(111)}}
```
