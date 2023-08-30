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
