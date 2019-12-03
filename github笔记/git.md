# 在Linux 上使用git
1. 安装git
```
sudo apt-get install git
```
2. 创建版本库
(1).　创建一个git文件
```
mkdir learngit
cd learngit
pwd
//最后这行是 pwd 运行结果
/Users/michael/learngit
```
(2). 初始化文件
```
//刚刚上一个步骤已经到达我们要用的文件夹了，现在只需要把文件夹初始化就可以了
git init
```
(3). 把文件添加到版本库中
```
//要先创建一个文件,比如我们这个文件叫read.txt
git add readme.txt
```
(4).　提交文件
```
git commit -m "wrote a readme file"
```
