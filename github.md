# 从远程库克隆
在当前目录下创建远程仓库
```
git clone git@github.com:tzwj1983/note-git.git
```

# 连接远程库
要关联一个远程库，使用命令 
```
格式
git remote add origin git@server-name:path/repo-name.git
具体
git remote add origin git@github:tzwj1983/note-git.git

```
关联后， 第一次推送master分支的所有内容。
```
git push -u origin master
```

每次本地提交使用命令,推送最新修改。
```
git push origin master
```
