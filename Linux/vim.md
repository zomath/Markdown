Fri Apr 26 08:37:46 CST 2019

# 按键说明
## 光标移动的方法
0 回到行首
$ 回到行尾
H 回到屏幕的第一行的第一个字符
M 回到屏幕中间哪一行的第一个字符
L 回到屏幕的最后一行的第一个字符
nG 到文件的第几列
n<ENTER> 光标向下移动n列
## 搜索与取代
/word 向光标之下寻找word
?word 向光标之上寻找word
n 重复前一个搜寻动作
N 反向重复前一个搜寻动作
:n1,n2s/word1/word2/g 将n1到n2行的word1全部替换为word2
:1,$s/word1/word2/g 第一行到最后一行的word1替换为word2
:1,$s/word1/word2/gc 加上一个c后，替换时候会让你确认
## 删除、复制与粘贴
x,X x向后删除，X向前删除
d1G 删除光标所在行到第一行的内容
dG 删除光标所在行到最后一行的内容
d$ 删除光标所在处到最后一个字符(在同一行内)
d0 删除光标所在处到第一个字符
y1G 复制光标所在行到第一行的内容
yG 复制光标所在行到最后一行的内容
p,P 粘贴到光标所在下一行，P粘贴到光标所在上一行
J 将光标所在和下一行合并在一行 
c 重复删除多个数据
u 复原前一个动作
[Ctrl]+r 重做上一个动作
. 重复前一个动作
## 进入取代编辑模式
r,R r取代光标所在字符一次，R会一直取代光标所在字符
## 命令行界面的储存、离开等指令
:w 保存
:w! 若文件为只读模式，则强制保存
:q 退出
:q! 不保存退出
ZZ 改动则保存离开，未改动则直接离开
:w [filename] 将文件保存为filename文件名
:r 将另外一个文件的内容添加到光标之后
:n1,n2 w [filename] 将n1到n2行内容保存为filename这个文件
:! command 执行系统命令
## vim环境变更
:set nu 显示行号
:set nonu 取消行号
## 区块选择
v 字符选择，光标经过的地方反白
V 行选择
[Ctrl]+v 区块选择
y 反白的地方复制
d 反白的地方删除
p 粘贴
