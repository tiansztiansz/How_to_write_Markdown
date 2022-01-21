# 编写Markdown文件
<!-- vscode-markdown-toc -->
* 1. [插入目录](#1)
* 2. [预览](#2)
* 3. [导出为pdf文件](#3)
* 4. [标题](#4)
* 5. [换行](#5)
* 6. [字体](#6)
* 7. [分隔线](#7)
* 8. [删除线](#8)
* 9. [下划线](#9)
* 10. [脚注](#10)
* 11. [列表](#11)
* 12. [区块](#12)
* 13. [代码](#13)
* 14. [链接](#14)
* 15. [图片](#15)
* 16. [表格](#16)
* 17. [键盘键](#17)
* 18. [转义](#18)
* 19. [公式和符号](#19)
	* 19.1. [参考文献](#20)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->


##  1. <a name='1'>插入目录</a>  
在VS Code的拓展中搜索`Markdown TOC`，安装拓展后，回到.md文件，光标指向文件开头，然后鼠标右键选择`命令面板`，在搜索框输入`Generate TOC for markdown`  
注意标题要命名为
```markdown
<a name='1'>插入目录</a>
```

##  2. <a name='2'>预览</a>  
`侧边预览`：打开VS Code，在.md文件中鼠标右键，然后选择“命令面板”，在搜索框处输入“Markdown: Open Preview to the Side” 。或者先选择.md文件，然后点击右上角的侧边预览图标。  
`全屏预览   `：
在VS Code中键入如下快捷键：   
<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>V</kbd>  







##  3. <a name='3'>导出为pdf文件</a>
在拓展处下载“Markdown PDF”，在.md文件中右键，即可看到导出为pdf文件的选项


##  4. <a name='4'>标题</a>
```markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```



##  5. <a name='5'>换行</a>  
“使用两个以上空格加上回车”  
或者“空一行”，



##  6. <a name='6'>字体</a>  
```markdown
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```



##  7. <a name='7'>分隔线</a>  
```markdown
***

* * *

*****

- - -

----------
```



##  8. <a name='8'>删除线</a>  
```markdown
~~BAIDU.COM~~
```


##  9. <a name='9'>下划线</a>  
```markdown
<u>带下划线文本</u>
```

##  10. <a name='10'>脚注</a>  
```markdown
创建脚注格式类似这样 [^RUNOOB]。
[^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！
```


##  11. <a name='11'>列表</a>    
`有序列表`
```markdown
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项
```



`无序列表`  
```markdown
1. 第一项
2. 第二项
3. 第三项
```  

`列表嵌套  `
```markdown
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```



##  12. <a name='12'>区块</a>  
```markdown
> 区块引用  
> 菜鸟教程  
> 学的不仅是技术更是梦想  
```

`区块嵌套  `
```markdown
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```


`区块中使用列表   `
```markdown
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项
```


`列表中使用区块  `   

在 > 前添加四个空格的缩进   
```markdown
* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项
```

##  13. <a name='13'>代码</a>  
反引号：英文输入法中键入键盘左上角处的  `  键  
```markdown
`printf()` 函数 
```


`代码区块`  
4 个空格或者一个制表符（Tab 键）  
或者用 ``` 

 




##  14. <a name='14'>链接</a>   
这里菜鸟教材指向某一网址   
```markdown
这是一个链接 [菜鸟教程](https://www.runoob.com)   
```
或者直接使用网址，即链接没有被赋予别名：  
```markdown
<https://www.runoob.com>  
```


`高级链接`   
通过变量来设置一个链接，变量赋值在文档末尾进行,有点类似参考文献的感觉  
```markdown
这个链接用 1 作为网址变量 [Google][1]  
这个链接用 runoob 作为网址变量 [Runoob][runoob]  
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/  
```


##  15. <a name='15'>图片</a>   
```markdown
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)
```
```markdown
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")  
```
```markdown
<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">  
```
```markdown
这个链接用 1 作为网址变量 [RUNOOB][1].
然后在文档的结尾为变量赋值（网址）

[1]: http://static.runoob.com/images/runoob-logo.png  

```

##  16. <a name='16'>表格</a>   
``` markdown
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |  
```

`对齐方式`  
```markdown
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |  
```

##  17. <a name='17'>键盘键</a>  
```markdown
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑  
```


##  18. <a name='18'>转义</a>  
```markdown
**文本加粗** 
\*\* 正常显示星号 \*\*  
```

以下这些符号前面加上反斜杠来帮助插入普通的符号   
```markdown
\   反斜线
`   反引号
*   星号
_   下划线
{}  花括号
[]  方括号
()  小括号
#   井字号
+   加号
-   减号
.   英文句点
!   感叹号  
```

##  19. <a name='19'>公式和符号</a> 
```markdown
$...$ 或者 \(...\) 中的数学表达式将会在行内显示。
```
```markdown
$$...$$ 或者 \[...\] 或者 ```math 中的数学表达式将会在块内显示。  
```
更多符号见：https://katex.org/docs/supported.html   
  




###  19.1. <a name='20'>参考文献</a>   
https://jingyan.baidu.com/article/60ccbceba8d4f464cbb19740.html  
https://www.runoob.com/markdown/md-advance.html   
