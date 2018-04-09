GitHub Flavored Markdown(GFM) 是对Markdown语法的扩展，在Markdown语法基础上增加了一些特性。由于自己在学习Markdown的使用时发现很多教程写得都不是特别简单明了，故自行整理出了一份教程。

[TOC]

## 标题
```markdown
语法：  
	标题名前加#（#后留一个空格，可加1-6个#代表不同级别标题）
代码示例：
	# 一级标题
	## 二级标题
	### 三级标题
	#### 四级标题
	##### 五级标题
	###### 六级标题
代码效果见下：
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题


## 文本

### 换行
```markdown
语法：
	在要换行处输入两个空格然后回车（直接只回车是没用的，不过可以回车两次，只是行间距会比较大）
代码示例：
	第一行文本（在这里输入两个空格然后回车）
	第二行文本
代码效果见下：
```
第一行文本  
第二行文本

### 文本样式
样式|语法|代码示例|代码效果
---|---|-------|-------
正常|无|`文本`|文本
斜体|`* *`或`_ _`|`*文本*`或`_文本_`|_文本_
粗体|`** **`或`__  __`|`**文本**`或`__文本__`|**文本**
粗斜体|`*** ***`或`___  ___`|`***文本***`或`___文本___`|___文本___
删除线|`~~ ~~`|`~~文本~~`|~~文本~~
`粗体、斜体、删除线可以和粗斜体那样混合使用。`


## 引用文本
```markdown
语法：
	引用的文本前加>（>后可不留一个空格，但建议留一个以便养成良好习惯）
代码示例：
	> 引用的文本
代码效果见下：
```
> 引用的文本（单行）


## 引用代码&&代码高亮
	语法：
		1.行内引用：引用的代码前后各加一个反引号`（英文输入法下，Tab键上面那个键）；
		2.区块引用：引用的代码块上下一行各加三个反引号`（英文输入法下，Tab键上面那个键）。
		3.代码高亮：引用的代码块上下一行各加三个反引号`，并在第一个三个反引号后加上语言标识符（如：javascript)。
	1.行内引用，代码示例：
		Use `git status` to list all new or modified files that haven't yet been committed.
	2.区块引用，代码示例：
        ```
        function test() {
          console.log("notice the blank line before this function?");
        }
		```
    3.代码高亮，代码示例：
    	```javascript
        function test() {
          console.log("notice the blank line before this function?");
        }
        ```
	代码效果见下：
1.行内引用：  
Use `git status` to list all new or modified files that haven't yet been committed.  
2.区块引用：
```
function test() {
  console.log("notice the blank line before this function?");
}
```
3.代码高亮:
```javascript
function test() {
  console.log("notice the blank line before this function?");
}
```
[查看GitHub支持代码高亮的所有语言](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)


## 链接

### 外部链接
```markdown
语法：
	[链接的描述](URL)
代码示例：
	[我的博客](http://www.honkerzhou.com/)
代码效果见下：
```
[我的博客](http://www.honkerzhou.com/)

### 内部链接
```markdown
语法：
	[链接的描述](#要跳到的标题名)
代码示例：
	[跳到表情处](#表情)
代码效果见下：
```
[跳到表情处](#表情)



## 列表

### 有序列表
```markdown
语法：
	数字后加一个小数点再加一个空格
代码示例：
	1. 第一天
	2. 第二天
	3. 第三天
代码效果见下：
```
1. 第一天
2. 第二天
3. 第三天

### 无序列表
```markdown
语法：
	减号或星号(*)后加一个空格（推荐用减号，可以少按一个Shift键）
代码示例：
	* 中国
	* 小明
	- 地板
代码效果见下：
```
* 中国
* 小明
- 地板

### 嵌套列表
```markdown
语法：
	和有序无序类似，主要是混合使用有序和无序
代码示例：
	1. 中国
	   - 北京
	   - 深圳
		 - 宝安区
		 - 福田区
代码效果见下：
```
1. 中国
   - 北京
   - 深圳
     - 宝安区
     - 福田区 

### 任务列表
```markdown
语法：
	减号加一个空格再加一个中括号再加一个空格（中括号中保留一个空格，如果完成了，就把中括号  中的空格改为字母x）
代码示例：
	- [x] 写Markdown语法总结
	- [ ] 月入百万
	- [ ] 环游世界
代码效果见下：
```
- [x] 写Markdown语法总结
- [ ] 月入百万
- [ ] 环游世界


## 表情
```markdown
语法：
	:表情代码:
代码示例：
	:shipit:
代码效果见下：
```
:shipit:
[表情代码查询表](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

