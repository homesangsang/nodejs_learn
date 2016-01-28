Node.js 异步变成的直接体现是回调   
下面分别列举阻塞代码和非阻塞代码  

### 阻塞代码   
```
 var fs = require("fs");
 var data = fs.readFileSync('filename');
 console.log(data.toString());
 console.log("程序执行结束");
```
### 非阻塞代码   
```
var fs = require("fs");
var data = fs.readFile('filename',function(err,data){
    if(err) return console.err(err);
    console.log(data.toString());
  });
console.log("程序执行结束！");
```

#### 理解上面两段代码
可以看出，fs.readFileSync("")是制定的使用阻塞的方式来读取文件，fs.readFile("".fun)是通过回调函数实现，\如果需要处理回调函数的参数，我们就需要写在回调函数内。\
