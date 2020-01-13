# Nand-to-Tetris

从零构建一台计算机

chapter1：
bug1:
在看视频教程尝试第一章的Xor CHIP时不能在project01里面使用哪个Xor CHIP模板。
因为仿真软件会读取文件内其他Nor And Or CHIP，但是这几个CHIP实际上还只是一个空的模板，
所以那个计算按钮不会被激活。但是如果在Project00内使用一个Xor CHIP，
仿真器就会调用内建的CHIP,在BuiltIn文件夹内，这个时候仿真的运行就没有问题。

bug2:
CHIP中的类似数组的变量从测试脚本中读取数据信息的时候是反向的，set[] = 10 ,set[1]==1,set[0]==0.

即set[0]是最右边的数据，set[maxNum]是最左边的数据。

bug3:CHIP输出变量的顺序不能改变。

bug4:中文分号会有空格，英文分号没有，但是两个分号长得一样。

bug5:对于in[num],这种取值的方法只能用在输入输出变量上，不能用在中间变量上。

bug6:CHIP中的变量默为0。可以直接使用一个变量。