

# Markdown 标

## 二级标题

### 三级标题



# Markdown 段落

Markdown 段落没有特殊的格式，直接编写文字就好，**段落的换行是使用两个以上空格加上回车**。



## **字体**

```
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```



*斜体文本*

**粗体文本**

__粗体文本__
***粗斜体文本***
___粗斜体文本___



## 分割线

```
***

* * *

*****

- - -

----------
```

***

---



## 删除线

```
~~~删除线~~~
```

~~删除线~~



## 下划线



```
<u>带下划线文本</u>
```

<u>带下划线文本</u>



## 脚注

```
[^要注明的文本]
```

创建脚注格式类似这样[^脚注]



# 列表

## 无序列表

无序列表使用星号(*****)、加号(**+**)或是减号(**-**)作为列表标记，这些标记后面要添加一个空格，然后再填写内容：

* 第一项
* 第二项
* 第三项



+ 第一项
+ 第二项
+ 第三项



- 第一项
- 第二项
- 第三项



## 有序列表

有序列表使用数字并加上 **.** 号来表示，如：

1. 第一项

2. 第二项

3. 第三项

   

## 列表嵌套

列表嵌套只需在子列表中的选项前面添加四个空格即可：

```
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```

1. 第一项
       - 第一项嵌套的第一个元素
       - 第一项嵌套的第二个元素
2. 第二项
       - 第二项嵌套的第一个元素
       - 第二项嵌套的第二个元素
3. 第三项
      - 第三项嵌套的第一个元素
      - 第三项嵌套的第二个元素



# 区块

Markdown 区块引用是在段落开头使用 **>** 符号 ，然后后面紧跟一个**空格**符号：

```
> 区块引用1
> 区块引用2
```

> 区块引用1
>
> 区块引用2
>
> 区块引用3



另外区块是可以嵌套的，一个 **>** 符号是最外层，两个 **>** 符号是第一层嵌套，以此类推：



> 最外层
>
> > 第一层嵌套
> >
> > > 第第二层嵌套



## 区块中使用列表

```
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项
```

> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项



## 列表中使用区块

```
* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项
```

* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
    
* 第二项



# 代码

## 段落中代码

如果是段落上的一个函数或片段的代码可以用反引号把它包起来（**`**），例如“

```
`printf()` 函数
```

`printf()` 函数

## 区块代码

1. 用 **```** 包裹一段代码，并指定一种语言（也可以不指定）：

```javascript
$(document).ready(function () {
    alert('代码');
});
```







# 链接

# 表格

# 高级技巧

## 支持的 HTML 元素

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。

目前支持的 HTML 元素有：`<kbd> <b> <i> <em> <sup> <sub> <br>`等 ，如：

```html
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
```

效果：

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑



##  转义

Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符：

```java
**文本加粗** 
\*\* 正常显示星号 \*\*
```

**文本加粗** 
\*\* 正常显示星号 \*\*

```html
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

## 公式

当你需要在编辑器中插入数学公式时，可以使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现。提交后，问答和文章页会根据需要加载 Mathjax 对数学公式进行渲染。如：

```
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
```

效果：

$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$



## 流程图

**1、语法介绍**

```nginx
%% 语法示例： ()圆角，[]方形，([])圆弧
graph LR
A[方形]
B(圆角)
C([圆弧])
D[[子程序]]
E[(圆柱:Database)]

F((圆形))
G>指向]
H{棱形}
I{{六边形}}
J[/平行四边形/] --> K[\平行四边形\]
L[/梯形\] --> M[\梯形/]
```

```mermaid
graph LR
A[方形] -->
B(圆角) -->
C([圆弧]) -->
D[[子程序]] -->
E[(圆柱:Database)] -->

F((圆形))
G>指向] -->
H{棱形} -->
I{{六边形}} -->
J[/平行四边形/] --> K[\平行四边形\]
L[/梯形\] --> M[\梯形/]
```

```mermaid
graph LR
A[实线] --> B[带箭头]
A[实线] --- C[不带箭头]
A[实线] -->|带文本|D[带箭头] --或--> E[带箭头]
A[实线] -- 带文本 --- F[不带箭头] --- |或| G[不带箭头]

```





**2、横向流程图源码格式：**

```nginx
​```mermaid
%% 语法示例： ()圆角，[]方形，([])圆弧
graph LR
A[方形] -->B(圆角)
    B --> C{条件a}
    C -->|a=1| D[结果1]
    C -->|a=2| E[结果2]
    F([横向流程图])
​```
```

效果图：

```mermaid
%% 语法示例： ()圆角，[]方形，([])圆弧
graph LR
A[方形] -->B(圆角)
    B --> C{条件a}
    C -->|a=1| D[结果1]
    C -->|a=2| E[结果2]
    F([横向流程图])
```

**3、竖向流程图源码格式：**

~~~nginx
```mermaid
%% 语法示例： ()圆角，[]方形，([])圆弧
graph TD
A[方形] --> B(圆角)
    B --> C{条件a}
    C --> |a=1| D[结果1]
    C --> |a=2| E[结果2]
    F([竖向流程图])
```
~~~

效果图：

```mermaid
%% 语法示例： ()圆角，[]方形，([])圆弧
graph TD
A[方形] --> B(圆角)
    B --> C{条件a}
    C --> |a=1| D[结果1]
    C --> |a=2| E[结果2]
    F([竖向流程图])
```



**4、标准流程图源码格式：**

~~~nginx
```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st->op->cond
cond(yes)->io->e
cond(no)->sub1(right)->op
```
~~~

效果图：

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st->op->cond
cond(yes)->io->e
cond(no)->sub1(right)->op
```



**5、标准流程图源码格式（横向）：**

~~~nginx
```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st(right)->op(right)->cond
cond(yes)->io(bottom)->e
cond(no)->sub1(right)->op
```
~~~

效果图：

```flow
st=>start: 开始框
op=>operation: 处理框
cond=>condition: 判断框(是或否?)
sub1=>subroutine: 子流程
io=>inputoutput: 输入输出框
e=>end: 结束框
st(right)->op(right)->cond
cond(yes)->io(bottom)->e
cond(no)->sub1(right)->op
```



## 时序图

**1、UML时序图源码样例：**

~~~nginx
```sequence
对象A->对象B: 对象B你好吗?（请求）
Note right of 对象B: 对象B的描述
Note left of 对象A: 对象A的描述(提示)
对象B-->对象A: 我很好(响应)
对象A->对象B: 你真的好吗？
```
~~~

```sequence
对象A->对象B: 对象B你好吗?（请求）
Note right of 对象B: 对象B的描述
Note left of 对象A: 对象A的描述(提示)
对象B-->对象A: 我很好(响应)
对象A->对象B: 你真的好吗？
```

**2、UML时序图源码复杂样例：**

~~~nginx
```sequence
Title: 标题：复杂使用
对象A->对象B: 对象B你好吗?（请求）
Note right of 对象B: 对象B的描述
Note left of 对象A: 对象A的描述(提示)
对象B-->对象A: 我很好(响应)
对象B->小三: 你好吗
小三-->>对象A: 对象B找我了
对象A->对象B: 你真的好吗？
Note over 小三,对象B: 我们是朋友
participant C
Note right of C: 没人陪我玩
```
~~~

```sequence
title: 标题：复杂使用
对象A->对象B: 对象B你好吗?（请求）
Note right of 对象B: 对象B的描述
Note left of 对象A: 对象A的描述(提示)
对象B-->对象A: 我很好(响应)
对象B->小三: 你好吗
小三-->>对象A: 对象B找我了
对象A->对象B: 你真的好吗？
Note over 小三,对象B: 我们是朋友
participant C
Note right of C: 没人陪我玩
```



**3、UML标准时序图样例：**

~~~nginx
```mermaid
%% 时序图例子,-> 直线，-->虚线，->>实线箭头
  sequenceDiagram
    participant 张三
    participant 李四
    张三->王五: 王五你好吗？
    loop 健康检查
        王五->王五: 与疾病战斗
    end
    Note right of 王五: 合理 食物 <br/>看医生...
    李四-->>张三: 很好!
    王五->李四: 你怎么样?
    李四-->王五: 很好!
```
~~~

```mermaid
%% 时序图例子,-> 直线，-->虚线，->>实线箭头
  sequenceDiagram
    participant 张三
    participant 李四
    张三->王五: 王五你好吗？
    loop 健康检查
        王五->王五: 与疾病战斗
    end
    Note right of 王五: 合理 食物 <br/>看医生...
    李四-->>张三: 很好!
    王五->李四: 你怎么样?
    李四-->王五: 很好!
```



## 甘特图

**1、甘特图样例：**

~~~nginx
```mermaid
%% 语法示例
        gantt
        dateFormat  YYYY-MM-DD
        title 软件开发甘特图
        section 设计
        需求                      :done,    des1, 2014-01-06,2014-01-08
        原型                      :active,  des2, 2014-01-09, 3d
        UI设计                     :         des3, after des2, 5d
    未来任务                     :         des4, after des3, 5d
        section 开发
        学习准备理解需求                      :crit, done, 2014-01-06,24h
        设计框架                             :crit, done, after des2, 2d
        开发                                 :crit, active, 3d
        未来任务                              :crit, 5d
        耍                                   :2d
        section 测试
        功能测试                              :active, a1, after des3, 3d
        压力测试                               :after a1  , 20h
        测试报告                               : 48h
```
~~~

```mermaid
%% 语法示例
gantt
dateFormat  YYYY-MM-DD
title 软件开发甘特图
section 设计
	需求                      :done,    des1, 2014-01-06,2014-01-08
	原型                      :active,  des2, 2014-01-09, 3d
	UI设计                    :         des3, after des2, 5d
	未来任务                   :         des4, after des3, 5d
section 开发
	学习准备理解需求            :crit, done, 2014-01-06,24h
	设计框架                   :crit, done, after des2, 2d
	开发                      :crit, active, 3d
	未来任务                   :crit, 5d
	耍												 :2d
section 测试
	功能测试                   :active, a1, after des3, 3d
	压力测试                   :after a1  , 20h
	测试报告                   : 48h
```



---

 结束

