# 移动app第2天

## 反馈问题
  - 速度;
  - 提交到服务器(github)
  - 上传博客(github博客)

## 回顾Git
- git是什么?
  + git 版本管理
- git 如何初始化一个git仓储
  + git init
- git 添加文件到暂存区
  +　git add [file]
- git提交暂存区文件到仓库中
  + git commit -m ""
- git status
  + 查看当前状态
- 查看日志:
  + git log
  +　git log --oneline

- git diff
  + 对不同版本的文件的不同

- 提交到远程服务器
  + git push [地址] master
- git remote add origin [地址]

- 搭建博客
  +　gh-pages



## Git继续
  - 使用ssh的方式上传代码

### 1.创建公钥私钥
  - 命令: `ssh-keygen -t rsa`
    ＋　这个命令会生成一个公钥和私钥，在ｃ盘用户目录下的.ssh目录。要把生成的公钥提供给服务器.
  - 不要重复使用这个命令：
    +　这个命令每一次生成的公钥私钥都不一样，

### 团队配合开发
    1. 初始化一个仓储，提交到远程服务器
    2. 从远程服务器下载仓储.
    3. 修改代码添加功能，
    4. 然后再提交到服务器（需要在本地先提交）

    *在团队开发中，一定要先拉再提交,push之前需要先pull一下*;
      - git pull [地址] [分支名].



### 从远程服务器拉取时出现冲突。
  - 如果遇到冲突，需要自己手动去处理冲突，选择想要保留的代码。
  - 如果解决冲突的时间太长，这个期间已经有个再次提交，我们需要再一次的pull代码。

### git使用流程
  - 1.新建文件夹，在文件夹中使用命令：`git init`初始化一个空的仓储
    ＋　这一步会在当前目录创建一个隐藏的.git文件夹
  - 2.开始写我们的项目，就在这个文件夹(.git同级目录)中写，写的时候就像我们之前一样去写。
  - 3.每次写完一个功能需要添加到暂存区
  - 4.把暂存区的代码提交到仓库。
  - 4.5如果，服务器仓储不是空的，我们需要先拉取到本地，然后解决冲突。
  - 5.把本地仓库里的代码提交到远程服务器
      + https
      + ssh
  - 6.继续更改我们的代码.
  - 7. 添加到暂存区，然后提交到本地仓库
  - 8.先pull，有冲突就解决冲突， 再提交到远程服务器。
  - 9.终于做完了

## bower
  - .bowerrc
    {
      "directory":"lib"
    }
  - 

## 开发问题
  - html,js ,css

## browser-sync
  - 用于浏览器刷新。
  - 安装:`npm install borwoser-sync -g`

  - 需要全局安装
  - 使用的命令:
    +`browser-sync start --server --files "./index.html" `
    + files参数的内容可以以逗号分割,*.html表示所html;
      css/*.css表示css目录下所有css   js/*.*

### browser-sync
  - 多浏览器兼容性同测试。

### 5.1.Gulp简介
- 链接：
    + [官网](http://gulpjs.com/)
    + [中文网](http://www.gulpjs.com.cn/)

