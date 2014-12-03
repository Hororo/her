her
===

Hao123 前端开发工具
基于FIS[http://fis.baidu.com/]

##安装使用##

###1.安装Her###
```
git clone https://github.com/hao123-dev/her.git
cd her
npm install
```
添加bin目录到环境变量

###2.安装her-pc-demo和her-smarty-plugin###
```
git clone https://github.com/hao123-dev/her-pc-demo
git clone https://github.com/hao123-dev/her-smarty-plugin
```
将her-smarty-plugin/plugin目录复制到her-pc-demo/common
```
cp -r her-smarty-plugin/plugin her-pc-demo/common
```

###3.发布her-pc-demo###
```
cd her-pc-demo/common
her release -c
cd ../home
her release -c
```
###4.启动her-server###
（需要java和php-cgi环境，安装方法见 http://fis.baidu.com/docs/api/cli.html#fis%20server%20%3Ccommand%3E%20%5Boptions%5D
```
her server init
her server start -p 8089
```
(用8089端口是为了防止与fis server默认的8080端口冲突)
浏览器将打开127.0.0.1:8089端口，即可看到her-pc-demo
