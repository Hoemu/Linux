# 使用`g++`编译`cpp`文件

1. 如果没有`g++`程序，需要下载安装，如下：
```
sudo apt install update
sudo apt install build-essential      //此步骤未安装其编译软件所必须的开发库和工具
sudo apt-get install manpages-dev     //安装 GNU/Linux 的开发手册
gcc --version 			      //查看当前 gcc 编译器是否安装
sudo update-alternatives --config gcc //修改默认的 gcc 版本
sudo apt install gcc-7 g++-7 	      //最后的数字是版本
```
