# Reference
Documents reference

#Issues
vlookup，查找数据出错，#NA
原因：
在vlookup函数查找过程中，文本型数字和数值型数字会被认为不同的字符。所以造成无法成功查找。

解决方案：
如：查找为数字，被查找区域为文本型数字。
把查找的数字在公式中转换成文本型，然后再查找。即：=VLOOKUP(A9&"",A1:D6,2,0)
若：查找格式为文本型数字，被查找区域为数值型数字。
把文本型数字转换成数值型。即：=VLOOKUP(A9*1,A1:D6,2,0)

其他错误类型及解决方法参考：http://www.officezhushou.com/vlookup/3887.html
