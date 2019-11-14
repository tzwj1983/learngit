# 创建SSH Key
- 查看在用户主目录下如果有.ssh目录且子目录有id_rsa和id_rsa.pub这两个文件。如果没有，打开Shell（Windows下打开Git Bash Here），创建SSH Key：
```
ssh-keygen -t rsa -C "youremail@example.com" 
```
具体操作时"youremail@example.com" 换成自己的邮箱地址。
- 登陆GitHub，打开“Account settings”-“SSH Keys”-“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容。
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
拉取当前分支最新代码
```
git pull
```
