﻿# ES6
### reduce
```
    <!DOCTYPE html>
    <html>
    	<head>
    		<meta charset="UTF-8">
    		<title></title>
    	</head>
    	<body>
    		<script type="text/javascript">
    			/*
    				Array.reduce(fn,init)
    
    				参数
    					function(addInit,item,index,arr)
    						addInit:上一次调用回调返回的值，或者是提供的初始值
    						item:数组中正在处理的元素
    						index:数组中正在处理的元素索引，如果提供了 init，从0开始，否则从1开始
    						arr:整个数组
    						
    					init:可选项
    						其值用于第一次调用 callback 的第一个参数。
    						如果没有设置初始值，则将数组中的第一个元素作为初始值。
    						空数组调用reduce时没有设置初始值将会报错。
    						
    				返回值
    					函数累计处理的结果
    			*/
    
    			let arr = [10,30,50,70];
    			let result = arr.reduce((addInit,item,index)=>{
    				//console.log(addInit,item,index)
    				return addInit+item;
    			})
    			console.log(result)
    			
    		</script>
    	</body>
    </html>
```
### 图示

![reduce](https://i.loli.net/2017/09/23/59c630e8b55ad.jpg)
