n1 -eq n2 检查n1是否与n2相等
n1 -ge n2 检查n1是否大于或等于n2
n1 -gt n2 检查n1是否大于n2
n1 -le n2 检查n1是否小于或等于n2
n1 -lt n2 检查n1是否小于n2
n1 -ne n2 检查n1是否不等于n2

expr 命令操作符

ARG1 | ARG2
ARG1 & ARG2
ARG1 < ARG2
ARG1 <= ARG2
ARG1 = ARG2
ARG1 != ARG2
ARG1 >= ARG2
ARG1 > ARG2
ARG1 + ARG2
ARG1 - ARG2
ARG1 * ARG2
ARG1 / ARG2
ARG1 % ARG2
STRING : REGEXP
match STRING REGEXP
substr STRING POS LENGTH
index STRING CHARS 
length STRING 
+ TOKEN (EXPRESSION)

如果ARG1既不是null也不是零值，返回ARG1；否则返回ARG2
如果没有参数是null或零值，返回ARG1；否则返回0
如果ARG1小于ARG2，返回1；否则返回0
如果ARG1小于或等于ARG2，返回1；否则返回0 
如果ARG1等于ARG2，返回1；否则返回0
如果ARG1不等于ARG2，返回1；否则返回0
如果ARG1大于或等于ARG2，返回1；否则返回0
如果ARG1大于ARG2，返回1；否则返回0
返回ARG1和ARG2的算术运算和
返回ARG1和ARG2的算术运算差
返回ARG1和ARG2的算术乘积
返回ARG1被ARG2除的算术商
返回ARG1被ARG2除的算术余数
如果REGEXP匹配到了STRING中的某个模式，返回该模式匹配
如果REGEXP匹配到了STRING中的某个模式，返回该模式匹配
返回起始位置为POS（从1开始计数）、长度为LENGTH个字符的子字符串
返回在STRING中找到CHARS字符串的位置；否则，返回0
返回字符串STRING的数值长度 
将TOKEN解释成字符串，即使是个关键字
返回EXPRESSION的值
