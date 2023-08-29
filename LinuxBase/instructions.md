- ## 网络
1. 拨号连接`sudo pppoeconf`
***
- ## 软件
1. 查看所有软件 `dpkg --list`　或　`dpkg -l`
2. 删除软件 
`sudo apt-get --purge remove[软件名称]` <br>
  (--purge是可选项，写上这个属性是将软件及其配置文件一并删除)<br>
3. 安装 git `audo apt install git`
4. 自带编辑器`nano`
***
- ## 文件
1. 创建文件 `touch 文件名称`
2. 查看当前位置 `pwd`
3. 查看文件夹所有下信息 `ll`，当然，也可以使用`ls`来查看信息，两者不同的是`ll`是纵向查看信息，包括了所有的文件信息（如文件日期），而后者`ls`则只是列出文件信息，不包括隐藏文件，如果需要列出隐藏文件，则需要使用这个指令`ls -a`.
4. 改变路径 `cd /文件路径`
5. 删除文件 `rm`
6. 删除目录 `rm -rf 目录名称`
7. 剪切粘贴文件/也可以完成修改文件名称 `mv`
8. 编辑文件 `vi`
9. 复制文件 `cp`
10. 创建一个文件夹`mkdir 文件夹名称`
11. 查看文件 `cat fileName`，也可以使用`shell`脚本进行查看
### 写文件 
`s`, `i`
#### 退出
1. 按　`esc`
2. 保存 `:wq` ,不保存 `:q!`
### 设置文件信息
1. 设置为隐藏文件:一般设置隐藏文件为前缀加`.`，可保证当前文件为隐藏

```
如：mv filename .filename
```
***
- ## 系统
1. 查看硬盘剩余空间 `df -h`
2. 打开进程 `ps -a`
3. 返回上一级 `cd`
4. 立刻关机 `init 0`
5. 获取系统root权限 `sudo nautilus` 或者：`sudo su`，都是可以获取系统权限的
6. 列出文件系统的整体磁盘使用量 `df`
7. 检查磁盘 `fsck`
8. 重启电脑`reboot`
- ## 其他
1. 返回上一级`cd ..`
2. 返回`home`目录`cd ~`

## 用户权限
### chmod 命令
1. `chmod` 命令全称 `change mode`，权限对应值如下：
```
u: rwx = 7
g: rx  = 5
o:  r- = 4
```
其中文件权限：读（r），写（w），执行（x）

2. 用户的创建和删除
创建用户指令: `useradd  -m userName`
删除用户指令：`sudo userdel userName`，有时候会出现当前用户线程，那么需要先单独停止线程，`sudo kill -9 process_id(PID)`，然后再使用`sudo userdel userName`，最后删除在`home`下的用户文件夹即可删除用户.

