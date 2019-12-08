# 在Linux 上使用git

1. 安装git
```
sudo apt-get install git
```
2. 创建版本库<br>
```
(1).　创建一个git文件
mkdir learngit
cd learngit
pwd
//最后这行是 pwd 运行结果
/Users/michael/learngit

(2). 初始化文件
//刚刚上一个步骤已经到达我们要用的文件夹了，现在只需要把文件夹初始化就可以了
git init

(3). 把文件添加到版本库中
//要先创建一个文件,比如我们这个文件叫read.txt
git add readme.txt
//当然 git add 可以加入多个文件，我们只需要在后面再添加就可以了

(4). 提交文件
git commit -m "wrote a readme file"
//这样做是为了告诉git 我们把文件提价到仓库里面了
```
3. 查看历史记录
```
(1). 查看历史提交
git status

(2). 查看历史修改
git diff 文件名称
//这个命令是只在我们还未提交上git 的时候可以查看我们修改的地方

(3). 查看历史版本
git log
//在每一次提交都自己写一个版本【git add 文件】【git commit -m "版本信息"】

(4). 退回以前的版本
git reset --hard HEAD^
HEAD 指的是当前版本，而 HEAD^ 是上一个版本，HEAD^^ 是上上个版本，但是要第100个版本可以直接写 HEAD~100

(5). 退回以前版本后再次返回新版本
git relog //记录你的每一次命令，然后查看新版本的最起前面的编号(commit_id)
然后输入 git reset --hard commit_id

(5).　丢弃工作区的修改
git checkout -- readme.txt
(6). 把暂存区的修改撤销掉，重新放回工作区
git reset HEAD readme.txt

```
[(参考廖雪峰git教程)](https://www.liaoxuefeng.com/wiki/896043488029600)
