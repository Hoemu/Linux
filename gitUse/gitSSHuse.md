### 1. 配置用户和邮箱

```
 git config --global user.name "你的用户名"

 git config --global user.email "你的邮箱"
```

不输入修改自己的用户名和邮箱可以查看自己已经输入的信息，如：

```
git config --global user.name
userName
git config --global user.email 
email@gmil.com
//当然，你也可以选择使用如下命令查看
git config --global --list
```

也可以通过修改全局配置文件 

```
vim ~/.gitconfig (通过输入此行命令打开配置文件，列如下方就是打开的文件)
---------------------------------------------------------------------------------------------
[filter "lfs"]
        smudge = git-lfs smudge -- %f
        process = git-lfs filter-process
        required = true
        clean = git-lfs clean -- %f
[user]
        name = obob
        email = lnz@123.com
[gui]
        recentrepo = E:/.../.../.../.../...
[core]
        editor = \"D:\\...\\... ... ...\\... ... ...\\.......\" --wait
----------------------------------------------------------------------------------------------
```

只需要修改 `[user]`中的`name`和`email`即可，然后按冒号键`:`，再按`w`和`q`（按照顺序）

 ### 2. 生成ssh

 * `cd ~/.ssh`命令进入`ssh`文件，然后输入`ls`查看是否有 `ssh`的相关文件文件

    * 如文件：`id_rsa` &nbsp; `id_rsa.pub`

 * 如果不存在`ssh`文件，输入`ssh-keygen -t rsa -C "your_email@youremail.com"`命令，生成`ssh`相关文件

  * 在后面可以填入密码，也可以不填入密码
  
    填入密码的反馈语句大概是这样的：

 ```
Enter passphrase (empty for no passphrase): 你的密码(直接按Enter键跳过)

Enter same passphrase again: 再次输入你的密码(直接按Enter键跳过)
 ```
* 查看生成的公钥

    *  `cat id_rsa.pub`
    
    * 然后吧显示出来的复制下来

* 打开`github`，点击你的头像，然后想选择`settings`，找到`SSH and GPG keys`这一栏.

    * 选择`New SSH key`，随便填写一个`Title`，然后把公钥复制在下面的框中.

### 3. 修改`git`的`remote url`

* 查看当前仓库的`remote url`使用命令：`git remote -v`

* 修改为`ssh`使用命令`git remote set-url origin 你自己当前仓库的ssh地址`




[参考文档](https://www.cnblogs.com/superGG1990/p/6844952.html)
