# 写一个简单 `shell` 脚本
1.  使用 `cat > shellName.sh` 回车，写入`shell`语句，如下所示:
```shell
cat > Hello.sh
#接下来这一行是输入代码
echo "Hello, world!";
#Ctrl + D 返回目录
```
2. 输入 `chmod u+x Hello.sh`，然后输入`sh Hello.sh`，就会有输出内容了，第一个脚本就此完成!

3. 变量的使用
```
VAR="abcd"
echo $VAR
```
如上，会输出`VAR`里面的值`abcd`(注意，变量的等号左右不能有空格！

4. 在`linux`使用脚本运行`cpp`程序

	1). 先准备一个`cpp`程序，我们可以把它命名为`service.cpp`
	2). 再写一个`.sh`脚本,假设`.sh`脚本名称为`run.sh`，如下：
		```
		cat > run.sh
		#! /bin/bash
		command g++ service.cpp -o service
		./service
		```
	3). 执行`.sh`文件: `sh run.sh`
5. `find`和`grep`
	1). `find`一般以文件属性的方式进行查找
	2). `grep`一般以文件内容的方式进行查找，如下：
		```
		grep *.cpp   	     //查找当前目录下的所有 .cpp 为后缀的文件
		grep string fineName //查找 fileName 下的 string 字符串
		```
