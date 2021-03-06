# 批处理问题件发邮件教程 

## 功能介绍
* 在excel中点击链接就可以快速的发送邮件
* 能够根据**问题类型**选择不同的话术

## 使用方法

1. 登录[erp系统](http://szerp.stosz.com:8080/Admin/Index/index)，在问题件处理中导出问题件excel表格
2. 将编辑好的函数[function]复制到相应的单元格中（U1）
3. 下拉U1单元格，使U列都填充
4. 点击相应的单元格即可发送邮件

## 使用原理

* **HYPERLINK** 超链接函数，可以设置相应的超链接对象
* **CONCATENATE** 字符串拼接函数，可以对相应的文字拼接
* **IF** 条件选择函数，可以根据不同的条件设置不同文字内容
* 邮件链接格式为 mailto：[邮箱]?subject=[主题]&body=[邮件内容]
* 最终函数内容[function.txt]，可以根据自己的需要修改相应的话术


## 注意事项

* 在使用前请将Foxmail设置为默认的邮箱
* 在使用过程中可能会出现乱码的情况，请手动复制相应的字符
* 请不要随意更改导出的数据，否则会导致失败
* 在将函数复制到单元格后会出现函数内容太多遮盖了下拉点，这边可以调高第一行的高度即可