# 一、安装
1. 输入 vim
2. 按照提示做就行了

# 二、使用
1. 编写一个文件 "vim 文件名称"
2. 写文件 "i" 或者 "s"
# 三、退出
1. 保存退出：<br>
      先按 "ESC" 然后输入 ":wq"
2. 不保存退出:<br>
      先按 "ESC" 然后输入 ":q!"<br>
# 三、配置 vim 
1. 在终端输入 “vim~/.vimrc”
2. 设置:<br>
(1). 改变代码的颜色 "syntax on"<br>
(2). 设置行号 "set number"<br>
(3). 支持鼠标 "set mouse=a"<br>
(4). 按下 Tab 键时，Vim 显示的空格数 "set tabstop=2"<br>
(5). 按下回车键后，下一行的缩进会自动跟上一行的缩进保持一致 "set autoindent"<br>
(6). 高亮显示当前行 "set cursorline"<br>
(7). vim命令自动补全 "set wildmenu"<br>
(7). 显示光标位置 "set ruler"
# 四、移动光标
1. 基本光标移动
     
     `h`：向左移动
     
     `l`：向右移动
     
     `j`：向上移动
     
     `k`：向下移动
     
2. 移动光标 "行号gg"
3. 删除一行 "cc"
4. 删除两行 "c2c"
5. 恢复 "u"
6. 复制 "p"
7. 一次向右跳一个单词的距离 "w"
8. 一次向左跳一个单词的距离 "B"
***
[更多操作](https://www.cnblogs.com/write-hua/p/7697762.html)
# 五、删除
1. 按　[ESC] 竟然命令行模式，再按　[1,$d]　就全删除啦
