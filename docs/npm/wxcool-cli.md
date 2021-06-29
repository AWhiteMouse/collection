# wxcool-cli

> 已停止更新。

### 项目描述

一款搭建原生小程序项目的脚手架。

使用时，只需要根据命令行的提示输入`description`、`author`、`appid`字段，即可快捷生成自己的原生小程序可执行项目。

### 运行原理

1. 通过一些第三方包（详见[依赖](#依赖)）在命令行中引导用户输入`description`、`author`、`appid`等信息；
2. 下载[项目模板](https://github.com/AWhiteMouse/WxCool)；
3. 将用户输入的信息插入到模板项目的`project.config.json`文件中；
4. 引导用户进入项目文件夹安装依赖并启动项目。

项目模板中使用了 `Gulp` 作为构建工具，`Gulp` 主要完成了以下功能：

+ 支持less。将less编译成wxss文件
+ 压缩。压缩JS、WXSS、JSON、WXML等文件，减少小程序包体积
+ 支持压缩图片，将图片转成base64格式
+ 支持在开发环境下进行热更新
+ 支持JS文件的ESLint校验
+ 支持Mock数据
+ 支持自动添加-webkit-前缀
+ ……

### 依赖

`chalk`、`commander`、`download-git-repo`、`handlebars`、`inquirer`等

### 项目地址

[wxcool-cli](https://www.npmjs.com/package/wxcool-cli)
