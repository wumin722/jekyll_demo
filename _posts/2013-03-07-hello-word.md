---
layout: default
title: 第一次记录
---
第一次记录
=============
刚放完假回到学校，总不知道要干啥。从网上看到有人用markdown写作，也就学着试试。

- Item  一来可以记录行为，以后数据能拿来分析
- Item  同时记录某些要点省得以后忘了，又要重新开始

关于git
------------
几个月前就开始用git了，但至今还没搞清楚到底怎么用。看了别人的介绍，大概有下面几步

1. 初始化
```
git init
```
2. 添加或着删除文件
```
git add/delete file
```
3. 评论更新
```
git commit -m 'first commit'
```
4. 连接github并且提交
```
git remote add origin git@github.com:defnngj/hello-world.git   //连接远程github项目  
git push -u origin master   //将本地项目更新到github项目上去
```

可能出现的问题
-------------
1. 在执行
```
$ git remote addorigin git@github.com:defnngj/hello-world.git
```
错误提示：fatal: remote origin already exists.

解决办法：
```
$ git remote rm origin
```
然后再执行：
```
$ git remote add origin git@github.com:defnngj/hello-world.git 
```
就不会报错误了

 

2. 在执行
```
$ git push origin master
```
错误提示：error:failed to push som refs to.......

解决办法：
```
$ git pull origin master //先把远程服务器github上面的文件拉先来，再push 上去。
```
如果服务器上和本地是不同的分支则
```
$ git pull origin 分支名
```
如果还不行则
```
$ git push -f //强行提交
```
********
参考网址[博客园][id].
[id]:http://www.cnblogs.com/fnng/archive/2011/08/25/2153807.html
