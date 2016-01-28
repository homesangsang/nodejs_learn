### REPL(交互解释器)   
REPL(Read Eval Print Loop : 交互解释器)，简单的讲就是终端里的配置的node这个程序，可以解释文件，也可以一条一条的解释执行javascript   
特点：   
* 可以直接进行简单的数学运算   
* 可以使用变量   var demo = 10 
* 多行表达式 
 ```
  do {
  ...
  ...
  ...}while();
```
* 下划线变量:可以使用下划线获取表达式的计算效果   
```
  var x = 10;
  var y = 20;
  x+y;
  var sum = _;
  console.log(sum);
```   
### REPL命令   
* ^c 退出当前终端  
* ^c两次 退出Node REPL  
* ^d 退出Node REPL   
* tab 列出当前命令   
* .help 列出使用命令   
* .break  退出多行表达式   
* .clear  退出多行表达式  
* .save filename 保存当前的Node REPL回话到指定文件，在当前目录下  
* .load filename 载入当前的Node REPL回话的文件内容   
