---
layout:     post
title:      Github命令速查表
subtitle:   Github命令
date:       2018-09-17
author:     Chauency
catalog: 	 true
tags:
    - Github
---

> *学习使用Github已有三年，但总是间隔性地使用，很多常用的基本命令都无法凭记忆打出来，每次都是网页百度OR翻看笔记，实在有点麻烦，是时候整理一下Github常用的命令了。--2019-09-17*

### 初始化本地git仓库
```shell
git init
```

### 本地仓库和远程仓库关联
``` 
git remote add origin git@github.com:chauency/**.git
```

### 远程库和本地库不一样导致push失败
``` 
git pull origin master --allow-unrelated-histories
```
### 将本地仓库的内容oush到远程仓库
``` 
git push [-u] origin master
```
第一次push需要添加参数-u

### 工作区的修改更新到暂存区
1. 直接列出具体文件  
```
git add file2.txt file3.txt
```
2. 提交所有修改和新建的文件（不包含删除的)    
```
git add .
```
3. 提交所有修改的文件（不包含新建的）  
```
git add -u
```
4. 提交所有的改动（修改+新建+删除）  
```
git add A
```

### 暂存区的内容更新到本地仓库
```
git commit -m "description of the modification"
```
