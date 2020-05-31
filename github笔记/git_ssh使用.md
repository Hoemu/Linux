[参考文档](https://www.cnblogs.com/superGG1990/p/6844952.html)

### 1. 配置用户和邮箱

  git config --global user.name "你的用户名"
  
  git config --global user.email "你的邮箱"
  
 ## 生成ssh
 
 * `cd ~/.ssh`命令进入`ssh`文件，然后输入`ls`查看是否有 `ssh`的相关文件文件
 
  * 如：`id_rsa`  `id_rsa.pub`
 
 * 如果不存在`ssh`文件，输入`ssh-keygen -t rsa -C "your_email@youremail.com"`命令，生成`ssh`相关文件
 
  * 在后面可以填入密码，也可以不填入密码
  
 大概是这样的
 
```
Enter passphrase (empty for no passphrase): 你的密码

Enter same passphrase again: 再次输入你的密码
```
