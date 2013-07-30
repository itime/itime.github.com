---
published: false
---

RequireJS快速入门
=

####语句解释

|语句|解释|示例
|-|-|
|`define`|定义一个模块|[define](#define)
|`require`|加载模块|[require](#require)
|`data-main="js/main"`|定义加载入口文件`main.js`|
|||



#####define示例：  {#define}
	
``` 
define( ['wojilu.test1'], function( t1 ) {
	return {
	NewTest : function() { t1.MyTest();}
   };
});
```

#####require示例： {#require}

```
require(["aModule", "bModule"], function() { 
    myFunctionA(); // 使用 aModule.js 中的函数 myFunctionA
    myFunctionB(); // 使用 bModule.js 中的函数 myFunctionB
}); 

```
