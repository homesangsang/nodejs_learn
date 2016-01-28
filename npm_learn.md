### npm学习笔记    

简介： npm是一个随nodejs自动安装的包管理工具，能解决nodejs代码部署到服务器上的很多问题，应用如下：   
* 允许用户从npm服务器上下载别人编写的第三方包到本地  
* 允许用户从npm服务器下载并安装别人编写的命令行程序到本地
* 允许用户将自己编写的包或命令行工具上传到npm服务器中供别人使用

#### 常用命令：
```
  mpm -v //显示版本号   
  sudo npm install npm -g //通过命令升级npm，-g表示全局安装   
  npm install <Module Name> [-g]//安装软件包,-g表示全局安装  
  npm ls [-g] //查看安装模块，带参数表示查看全局安装的模块   
  npm uninstall <Module Name> //卸载指定的模块  
  npm update <Module Name>  //升级指定的 模块    
  npm search <Mdule Name>    //搜索指定模块   
  
  npm help <command> //可查看某条命令的详细帮助 eg:npm help install    
  
```
#### 本地安装   
* 将安装包放在./node_modules 下，
* 可以通过require() 来引入本地包    

### 全局安装   
* (linux下)将安装包放在 /usr/local下   
* 可以直接在命令行里运行使用   
* 不能通过require()来引入本地安装包   

