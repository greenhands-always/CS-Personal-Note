# 变量
## 定义
定义变量时不需要加 `$`
变量命名规则:
-   命名只能使用英文字母，数字和下划线，首个字符不能以数字开头。
-   中间不能有空格，可以使用下划线 _。
-   不能使用标点符号。
-   不能使用bash里的关键字（可用help命令查看保留关键字）。
## 使用
==使用(重新赋值不算)==一个定义过的变量，只要在变量名前面加美元符号即可，如：
```
your_name="qinjx"  
echo ${your_name}
```
$引用时加上花括号比不加更好,更加适合多种情况

## 删除变量
```
unset variable_name
```
unset不能删除只读变量
# 字符串
注意单引号的限制
-   单引号里的任何字符都会原样输出，单引号字符串中的变量是无效的；
-   单引号字串中不能出现单独一个的单引号（对单引号使用转义符后也不行），但可成对出现，作为字符串拼接使用。
双引号
- 双引号里可以有变量
- 双引号里可以出现转义字符