[参考文档](https://www.cnblogs.com/superGG1990/p/6844952.html)

### 1. 配置用户和邮箱

  git config --global user.name "你的用户名"
  
  git config --global user.email "你的邮箱"
  
 ### 2. 生成ssh
 
 * `cd ~/.ssh`命令进入`ssh`文件，然后输入`ls`查看是否有 `ssh`的相关文件文件
 
    * 如文件：`id_rsa` &nbsp; `id_rsa.pub`
 
 * 如果不存在`ssh`文件，输入`ssh-keygen -t rsa -C "your_email@youremail.com"`命令，生成`ssh`相关文件
 
  * 在后面可以填入密码，也可以不填入密码
  
    填入密码的反馈语句大概是这样的：
 
 ```
Enter passphrase (empty for no passphrase): 你的密码

Enter same passphrase again: 再次输入你的密码
```
* 查看生成的公钥

    *  `cat id_rsa.pub`
    
    * 然后吧显示出来的复制下来

* 打开`github`，点击你的头像，然后想选择`settings`，找到`SSH and GPG keys`这一栏.

    * 选择`New SSH key`，随便填写一个`Title`，然后把公钥复制在下面的框中.

### 3. 修改`git`的`remote rul`

* 查看当前仓库的`emote rul`使用命令：`git remote -v`

* 修改为`ssh`使用命令`git remote set-url origin 你自己当前仓库的ssh地址`

* 结束