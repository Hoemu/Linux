## 安装　MySQL 
在终端输入 [sudo apt-get install mysql-server]　即可安装
## 安装后修改默认密码
1. 安装完成后，进入 root用户可直接输入mysql 进入mysql 里面
2. 在mysql 里面输入 [show databases]，找到 msyql 这个数据库，[use mysql]使用这个数据库
3. 输入[update user set authentication_string=PASSWORD("你的密码") where user='root';] 
4. 再输入[update user set plugin="mysql_native_password";]
5. 最后输入[flush privileges;]
6. 退出 mysql 输入[quit];
7. 重启mysql 输入　[mysql -u root -p;]　会显示你输入密码，就完成了
## 用终端使用 MySQL
### 基本语法
1. 查看数据库: show databases;
