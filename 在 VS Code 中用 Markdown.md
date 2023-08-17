# 教程向: 在 VS Code 中用 Markdown 做「数字化」学习笔记

[![一只方橙](https://picx.zhimg.com/v2-485768f5d1bbcd8e0fddfbe796949593_l.jpg?source=172ae18b)](https://www.zhihu.com/people/xia-chong-yu-bing-34-67)

[一只方橙](https://www.zhihu.com/people/xia-chong-yu-bing-34-67)

喜欢一切有趣的东西。GitHub：OrangeX4

关注他

[公子小白](https://www.zhihu.com/people/baby-little-51)等 937 人赞同了该文章

**VS Code** 配上 **Markdown** 语言, 就能写出酷炫, 便捷, 且适应互联网的「数字化」学习笔记.



![img](https://pic4.zhimg.com/80/v2-9e0a1762c0f90f507c3fb5cd6a34878b_1440w.webp)



这个教程是我这段时间踩过各种各样的坑之后, 总结 VS Code 做学习笔记的最佳实践.

**如果你对在 VS Code 中做笔记有什么好的主意, 欢迎留下你的意见, 我会第一时间在教程中加入!**



## 环境搭配

### 安装 VS Code

前往 [官网](https://link.zhihu.com/?target=https%3A//code.visualstudio.com/) 下载 VS Code, 点击 `Download`, 就会自动开始下载:



![img](https://pic2.zhimg.com/80/v2-65432d031dd5b2d99a6a78f5becb4895_1440w.webp)



如果网速较慢, 你也可以在 [腾讯软件中心](https://link.zhihu.com/?target=https%3A//pc.qq.com/detail/16/detail_22856.html) 下载.

进入安装界面, 将选项全部勾选, 点 **下一步** 和 **安装**, 直到安装完成即可.

### 中文支持 (选做)

如果你不想看英文, 想要中文版本的 VS Code, 你可以安装一个中文支持插件. 虽然我个人不太喜欢, 但是每个人都有自己的喜好嘛.

打开 VS Code, 点击插件面板, 输入 `Chinese`, 选择出现的第一个插件进行 `Install` 安装.



![img](https://pic4.zhimg.com/80/v2-8d2c22cec01a715a2f035de69999e4ef_1440w.webp)



安装好后, 按照右下角提示重启 VS Code.



![img](https://pic1.zhimg.com/80/v2-a5af8faf9a404a1750fb887cd0fd4ce0_1440w.webp)



可以看出, 界面以及变为中文了.



![img](https://pic2.zhimg.com/80/v2-92e296eaa53b5940aaeebe16ec808f35_1440w.webp)



### 安装 Markdown 相关插件

为了良好的记笔记体验, 你需要安装和 Markdown 相关的 VS Code 插件:

你可以下载我整理的这个 Extension Pack, 它包括了下面这些插件:

- Markdown Preview Enhanced
- Markdown All in One
- Better Markdown & Latex Shortcuts
- Latex Sympy Calculator
- Python Brackets
- Orangex4 Snippets
- Paste Image
- Vscode Icons

就像安装中文支持那样操作, 点击插件面板, 搜索 `Markdown-Notes-Pack`, 点击 `Install` 进行安装, 可能会花一点时间.



![img](https://pic4.zhimg.com/80/v2-c5f60e9494fc02b6a8674e8465cb1523_1440w.webp)



## 第一个 Markdown 文件: Hello World!

### 新建笔记工作区

工作区是什么?

工作区就是一个文件夹, 在你做笔记的时候, 工作区应该是你的笔记的根文件夹.

例如, 我在 D 盘创建了一个文件夹 `D:\Notes`, 那么我的工作区就应该是这个 `D:\Notes` 文件夹.

你可以像我一样, 在 D 盘新建一个 `Notes` 文件夹, 并在 VS Code 中打开这个文件夹.



![img](https://pic3.zhimg.com/80/v2-bdbfdcec40397c7253eec67b04e6763a_1440w.webp)





![img](https://pic1.zhimg.com/80/v2-00f078a786cd4c6dc41de0ca3e0030d0_1440w.webp)



### 在工作区子笔记文件夹

我个人比较喜欢将笔记按照不同的课程放在不同的文件夹下, 比如在我们的 Markdown 学习之旅中, 我们可以先新建一个文件夹叫 `Learn`.



![img](https://pic3.zhimg.com/80/v2-e5b460e4d376c9c7163e2e8f512c4c2a_1440w.webp)





![img](https://pic2.zhimg.com/80/v2-c30e7615741ed3eed65441a60fa37c39_1440w.webp)



新建一个文件, 命名为 `test.md`, **注意后缀一定要是 `.md`!!!** 这样表明它是一个 **Markdown** 文件. 你的所有笔记文件都应该以 `.md` 作为后缀.



![img](https://pic2.zhimg.com/80/v2-13abf5b6bd3966927b6dea7f34eac6ed_1440w.webp)



### 写下第一行 Markdown 笔记

输入笔记内容:

```text
# Hello, World!
```

(注意, # 和 文本之间要**加入空格**!)

然后**按照先后顺序**按下快捷键 `Ctrl + K, V`, 然后在右边就会出现预览窗口.

(注意, 快捷键按下时要**连贯**, 并且按下 `V` 的同时**不用按** `Ctrl` 键!)



![img](https://pic4.zhimg.com/80/v2-cb29c8506f57b405526fd27997b579ff_1440w.webp)



如果正常地显示出了标题 "Hello, World!", 那么恭喜你, 第一个 Markdown 笔记写成功了!

## 修改预览窗口背景 (选做)

相信聪明的你已经发现了一个问题:

**为什么我的预览窗口是白色的, 太刺眼了! 为什么你的预览窗口和代码窗口颜色一样?**

诶, 别急, 这就告诉你. 这里的预览窗口的 **Markdown Preview Enhanced** 插件生成的. 你只需要修改一下这个插件的配置就可以了.

按下快捷键 `Ctrl + ,`, 就会打开设置窗口.

在搜索框输入 `Preview Theme`, 看见标题为 Preview Theme 的选项, 在下拉框中选择 `atom-dark.css`, 就能让预览窗口的颜色改变了.

(当然, 颜色还是和 VS Code 有一点差别, 就不要在意这些细节啦)



![img](https://pic3.zhimg.com/80/v2-45e9f6416764f8cce0e64e5b80620c22_1440w.webp)



## Markdown 语法

纯粹的 Markdown 语法其实非常简单, 70 行的语法介绍就可以写完.

```text
# 一级标题

## 二级标题

### 三级标题

每写完一个段落要隔一行空行.

就像这样, 隔了一行空行.

---

分割线

**重点加粗**

*斜体*

~~删除线~~

---

列表:

* 无序列表
  * 嵌套无序列表
  * 嵌套无序列表
* 无序列表
* 无序列表

1. 有序列表 1
   1. 嵌套有序列表 1
   2. 嵌套有序列表 2
2. 有序列表 2
3. 有序列表 3

---

引用文本:

> 引用别人说的话
> 就这样写
> By. OrangeX4

---

这是 `行内代码` 语法.

代码块语法:

''' python
print("Hello, World!")
'''

请将 ' 替换成 `.

---

[超链接名称](链接地址)

![图片提示语](图片地址)

---

表格:

| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| 内容 | 内容 |

---

注释:

<!-- 你看不见我 -->
```

### 标题

你可以用

```text
# 一级标题

## 二级标题

### 三级标题

段落.
```

或

```text
一级标题
=======

二级标题
-------
```

的方式表示标题, 个人更推荐前一种方式. (不用对齐, 强迫症福音!)

### 段落

```text
段落和段落之间要隔一行.

就像这样.
```

### 分割线

```text
三条横线 (或更多的横线) 表示分割线.

---

就像这样.
```



![img](https://pic2.zhimg.com/80/v2-35c44fb7437e3c4e676e0f0af8cd5045_1440w.webp)



### 加粗, 斜体和删除线

做笔记的时候, 我们常常会有这样的要求, "加粗, 斜体和删除线", 作为笔记的

```text
**重点加粗**

*斜体*

~~删除线~~
```

**Markdown Preview Enhanced 拓展功能:**

```text
==高亮==
```



![img](https://pic2.zhimg.com/80/v2-a81b2adc3d8820855e1c6a761d3bdb1d_1440w.webp)



**快捷键:**

选中文本之后, 按下 `Ctrl + B` 可以给选中文本加粗.

同理 `Ctrl + I` 可以让选中文本变为斜体.

### 列表

列表是记笔记时非常基本的元素, 在 Markdown 中, 可以用很方便的格式书写列表:

```text
* 无序列表
  * 嵌套无序列表
  * 嵌套无序列表
* 无序列表
* 无序列表

1. 有序列表 1
   1. 嵌套有序列表 1
   2. 嵌套有序列表 2
2. 有序列表 2
3. 有序列表 3
```

**Markdown Preview Enhanced 拓展功能:**

```text
任务列表:

- [x] 已经完成的事 1
- [x] 已经完成的事 2
- [x] 已经完成的事 3
- [ ] 仍未完成的事 4
- [ ] 仍未完成的事 5
```



![img](https://pic4.zhimg.com/80/v2-dceae97b65a98286e995a6f59b1989b3_1440w.webp)



**快捷键:**

要进行**缩进** (书写嵌套列表), 你可以使用 VS Code 的快捷键 `Ctrl + [` 和 `Ctrl + ]`.

这个快捷键可以将代码向左或向右进行缩进!

### 引用和代码

```text
引用文本:

> 引用别人说的话
> 就这样写
> By. OrangeX4

这是 `行内代码` 语法.

代码块语法:

''' python
print("Hello, World!")
'''

注意要将 ' 替换成 `.
```



![img](https://pic1.zhimg.com/80/v2-bdf324d9b4e6b5dc60337a4db3255a48_1440w.webp)



Markdown Preview Enhanced 拓展功能:

```text
代码行数的显示:

''' javascript {.line-numbers}
function add(x, y) {
  return x + y
}
'''

注意要将 ' 替换成 `.
```



![img](https://pic1.zhimg.com/80/v2-cfcbfe6cf86e1ecdd5707549f12215e8_1440w.webp)



### 超链接和图片

你可以用下面的语法插入超链接和图片:

```text
[超链接名称](链接地址)

![图片提示语](图片地址)

例如, 可以使用网址和图床:

[OrangeX4's Blog](https://orangex4.cool/)

![OrangeX's Avatar](https://orangex4.cool/images/icons/profile.jpg)

也可以在本地用相对地址:

[Other](other.md)

![OrangeX's Avatar](images/profile.jpg)
```



![img](https://pic3.zhimg.com/80/v2-5b8a57c7d28198550130504ffe21bad2_1440w.webp)



### 剪贴板图片插入

看了上面的插入图片语法, 也许你会觉得, **好麻烦啊**.

我就插入一张图片, 居然还要把图片上传到网上. 或者把图片保存到本地, 还要移动图片, 命名什么的.

就不能像 Word 那样, 直接**剪贴板粘贴图片**吗?

万能的 VS Code 当然可以做到类似的事!

其实, 使用你已经安装了的 **Paste Image** 插件就行.

不过在使用之前, 你要做一点小调整:

按下 `Ctrl + ,` 打开设置窗口, 输入 `Paste Image Path` 并搜索, 将框内的文本改成 `${currentFileDir}/images`.



![img](https://pic2.zhimg.com/80/v2-c35303b43639b37a18b8893e906d7435_1440w.webp)



注意标题是 **Paste Image: Path**, 不要弄错了!

设置好之后, 你就可以使用剪贴板粘贴功能了!

**按下快捷键 `Ctrl + Alt + V`**,

就能把图片自动保存到当前目录下, 并以正确的格式粘贴到当前的 Markdown 文件中.

### 表格

你可以很方便地在做笔记的时候加入表格:

```text
表格:

| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| 内容 | 内容 |
```

**Markdown Preview Enhanced 拓展功能:**

```text
拓展语法:

| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| >    | 内容 |

| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| ^    | 内容 |
```



![img](https://pic4.zhimg.com/80/v2-fe477e9335bbff718c658057a86e0307_1440w.webp)



**快捷键:**

自动表格对齐: `Shift + Alt + F`

### 注释

注释不会被渲染出来.

你可以随手做点草稿, 如果还想保留着, 但是不显示, 就可以按下**快捷键** `Ctrl + \` **将当前行注释 / 反注释**.

```text
注释:

<!-- 你看不见我 -->

<!-- 多行注释
就像这样 -->
```

有一点很重要的就是, **VS Code 会在你每次修改代码之后, 重新渲染一遍**.

**如果有很多很多的数学公式, 渲染会很慢**, 这时候有两个建议:

- **分成多个文件, 避免单文件过大!**
- **将你暂时不看的部分注释掉, 加快渲染速度!**

## 数学公式支持

Markdown 的数学公式吸纳了大部分的 Latex 语法, 你可以以一种简单的方式在 VS Code 中书写数学公式.

```text
行内公式: 

单位圆 $x^2+y^2=1$

公式块:

$$
\begin{cases}
x=\rho\cos\theta \\
y=\rho\sin\theta \\
\end{cases}
$$
```



![img](https://pic4.zhimg.com/80/v2-42be969f982a47db9a53e087232ac2c3_1440w.webp)



**VS Code 有着非常便捷好用的自动补全功能**, 只需要简单地打出你想打的内容的几个字母 (**乱序**也行), 再使用 `↑ ↓` 进行选择, 最后按下回车就可以打出你想要的内容.

再使用 **HyperSnips 插件**, 就能够写得飞快.



![img](https://pic3.zhimg.com/80/v2-17cd3912fe219cdd7c8696af431eb456_1440w.webp)



还有, **不要在公式内使用中文**, 除非是 `\text{中文}` (但是也不推荐)

### 1. 上标和下标

```text
上标 $x^2 + y^{12} = 1$

上标 $x_1 + y_{12} = 1$
```



![img](https://pic2.zhimg.com/80/v2-a527faa78367be526a55992ebfae09f9_1440w.webp)



**HyperSnips 自动扩展**：

```text
xsr  =>  x^{2}

xtp  =>  x^{...}

x1  =>  x_1

xii  =>  x_i

xsb  =>  x_{...}
```

### 2. 分式

```text
较小的行内行分数 $\frac{1}{2}$

展示型的分式 $\displaystyle\frac{x+1}{x-1}$
```

其中 `\displaystyle` 用于将行内展示转为块状展示.



![img](https://pic1.zhimg.com/80/v2-6068b9817b165318fbb44912601a1450_1440w.webp)



**HyperSnips 自动扩展**：

```text
1/  =>  \frac{1}{...}

(1 + 2)/  =>  \frac{(1+2)}{...}

//  =>  \frac{...}{...}
```

### 3. 根式

```text
开平方 $\sqrt{2}$

开 $n$ 次方 $\sqrt[n]{2}$
```



![img](https://pic4.zhimg.com/80/v2-7f43224f74cae008fa950a82252e0903_1440w.webp)



**HyperSnips 自动扩展**：

```text
hsq  =>  \sqrt{...}
```

### 4. 空格

数学公式中的 **空格和换行** 都会在编译时 **被忽略**，想要实现「空格」的效果，需要用特别的命令。

```text
紧贴 $a\!b$

没有空格 $ab$

小空格 $a\,b$

中等空格 $a\;b$

大空格 $a\ b$

quad 空格 $a\quad b$

两个 quad 空格 $a\qquad b$
```



![img](https://pic2.zhimg.com/80/v2-3d5d3d55a6cc7fa4108a3d72287ec509_1440w.webp)



### 5. 累加, 累乘和积分

```text
累加 $\sum_{k=1}^n\frac{1}{k}  \quad  \displaystyle\sum_{k=1}^n\frac{1}{k}$

累乘 $\prod_{k=1}^n\frac{1}{k}  \quad  \displaystyle\prod_{k=1}^n\frac{1}{k}$

积分 $\displaystyle \int_0^1x{\rm d}x  \quad  \iint_{D_{xy}}  \quad  \iiint_{\Omega_{xyz}}$
```



![img](https://pic2.zhimg.com/80/v2-107c58a00665db46695c759d10926ded_1440w.webp)



**HyperSnips 自动扩展**：

```text
sum  =>  \sum_{...}

prod  =>  \prod_{<n=1>}^{<\infty>} ...

int  =>  \int

dint  =>  \int_{<-\infty>}^{<\infty>} ... \mathrm{d}x
```

Tips：按下 Tab 键可以跳转光标。

### 6. 括号修饰

用 `\left` 和 `\right` 可以让括号适配内部大小

```text
圆括号 $\displaystyle \left(\sum_{k=1}^{n}\frac{1}{k} \right)^2$

方括号 $\displaystyle \left[\sum_{k=1}^{n}\frac{1}{k} \right]^2$

花括号 $\displaystyle \left\{\sum_{k=1}^{n}\frac{1}{k} \right\}^2$

尖括号 $\displaystyle \left\langle\sum_{k=1}^{n}\frac{1}{k} \right\rangle^2$
```



![img](https://pic3.zhimg.com/80/v2-2564e223b37d79424ff60ecf1ee4e5b6_1440w.webp)



**HyperSnips 自动扩展**：

```text
@(  =>  \left( ... \right)

@[  =>  \left[ ... \right]

@{  =>  \left\{ ... \right\}

@<  =>  \left< ... \right>

set  =>  \{ ... \}
```

### 7. 多行算式对齐

```text
居中:

$$
\begin{aligned}
y &=(x+5)^2-(x+1)^2 \\
&=(x^2+10x+25)-(x^2+2x+1) \\
&=8x+24 \\
\end{aligned}
$$

左对齐:

$
\begin{aligned}
y &=(x+5)^2-(x+1)^2 \\
&=(x^2+10x+25)-(x^2+2x+1) \\
&=8x+24 \\
\end{aligned}
$
```



![img](https://pic4.zhimg.com/80/v2-2ce4065baebaa934da5963574f65bce7_1440w.webp)



**HyperSnips 自动扩展**：

```text
ali  =>
\begin{aligned}
... \\
\end{aligned}
```

如果你安装了 `Better Markdown & Latex Shortcuts` 插件，你还可以按下 `Shift + Ctrl + Alt + C` 可以将行公式转为 aligned 环境。



![img](https://pic3.zhimg.com/80/v2-c763db4ac47b3eec91610a2e51b0aa7a_1440w.webp)



### 8. 方程组

```text
$$
\begin{cases}
k_{11}x_1+k_{12}x_2+\cdots+k_{1n}x_n=b_1 \\
k_{21}x_1+k_{22}x_2+\cdots+k_{2n}x_n=b_2 \\
\cdots \\
k_{n1}x_1+k_{n2}x_2+\cdots+k_{nn}x_n=b_n \\
\end{cases}
$$
```



![img](https://pic1.zhimg.com/80/v2-a085a39d41c0af5ded6b328907e662ec_1440w.webp)



**HyperSnips 自动扩展**：

```text
case  =>
\begin{cases}
... \\
\end{cases}
```

### 9. 矩阵

```text
矩阵:

$$
\begin{pmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{pmatrix}

\quad

\begin{bmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{bmatrix}
$$ 

行列式: 

$$
\begin{vmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{vmatrix}
$$
```



![img](https://pic3.zhimg.com/80/v2-8f249643b32b0fd0375dc8f8c8b40d86_1440w.webp)



**HyperSnips 自动扩展**：

```text
bmat2  =>  \begin{bmatrix} ... & ... \\ ... & ... \\\end{bmatrix}

vec2  =>  \begin{pmatrix} ... \\ ... \\\end{pmatrix}
```

tips：按下 Tab 键可以切换到下一个位置。

### 10. 特殊字符



![img](https://pic2.zhimg.com/80/v2-842b02c54dd7d8e0571609414e79bdc1_1440w.webp)



更多特殊符号可以 [上网查询](https://link.zhihu.com/?target=https%3A//oeis.org/wiki/List_of_LaTeX_mathematical_symbols)

可以搜索 "Latex 符号表"

**HyperSnips 自动扩展**：

```text
alpha  =>  \alpha

Sigma  =>  \Sigma
```

### 11. 公式编号与引用

```text
$$
x+2 \tag{1.2}
$$

$$
\begin{equation}
x^n+y^n=z^n
\end{equation}
$$

由公式 $(1.2)$ 可得到结论
```



![img](https://pic2.zhimg.com/80/v2-e602d10556b445efba976af2ee0b4209_1440w.webp)



### 12. 零碎的重要语法

- 点乘 `$\cdot$`, 叉乘 `$\times$`, 异或 `$\otimes$`, 直和 `$\oplus$`, 加减 `$\pm$`, 复合 `$\circ$`.
- 小于等于 `$\leq$`, 大于等于 `$\geq$`, 不等 `$\neq$`, 恒等 `$\equiv$`, 约等 `$\approx$`, 等价 `$\cong$`, 相似 `$\sim$`, 相似等于 `$\simeq$`, 点等 `$\doteq$`.
- 逻辑与 `$\land$`, 逻辑或 `$\lor$`, 逻辑非 `$\lnot$`, 蕴涵 `$\to$`, 等价 `$\leftrightarrow$`.
- 因为 `$\because$`, 所以 `$\therefore$`, 存在 `$\exist$`, 任意 `$\forall$`.
- 左小箭头 `$\leftarrow$`, 右小箭头 `$\rightarrow$`, 左大箭头 `$\Leftarrow$`, 右大箭头 `$\Rightarrow$`, 右长箭头 `$\xrightarrow[fgh]{abcde}$`.
- 属于 `$\in$`, 包含于 `$\subset$`, 真包含于 `$\subseteq$`, 交 `$\cap$`, 并 `$\cup$`, 空集 `$\empty$`
- 短向量 `$\vec{x}$`, 长向量 `$\overrightarrow{AB}$`, 上横线 `$\overline{p}$`.
- 无限 `$\infty$`, 极限 `$\lim$`, 微分 `${\rm d}$`, 偏导 `$\partial$`, 点求导 `$\dot{y}$`, 点二阶导 `$\ddot{y}$`, 变化量 `$\Delta$`, 梯度 `$\nabla$`.
- 横省略 `$\cdots$`, 竖省略 `$\vdots$`, 斜省略 `$\ddots$`.
- 常见函数 `$\sin$`, `$\cos$`, `$\tan$`, `$\arcsin$`, `$\arccos$`, `$\arctan$`, `$\ln$`, `$\log$`, `$\exp$`.



![img](https://pic1.zhimg.com/80/v2-1063f781baa2bed9e7ebb32428719650_1440w.webp)



**HyperSnips 自动扩展**：

```text
**  =>  \cdot
xx  =>  \times
otimes  =>  \otimes
<=  =>  \le
!=  =>  \neq
==  =>  \equiv
~~  =>  \thickapprox
sim  =>  \sim
land  =>  \land
lor  =>  \lor
bec  =>  \because
thr  =>  \therefore
EE  =>  \exists
AA  =>  \forall
inn  =>  \in
sse  =>  \subseteq
sqs  =>  \sqsubseteq
cap  =>  \cap
cup  =>  \cup
empty  =>  \empty
oo  =>  \infty
lim  =>  \lim_{<n> \to <\infty>}
dd  =>  \mathrm{d}
part  =>  \frac{\partial <V>}{\partial <x>}
Delta  =>  \Delta
nabla  =>  \nabla
...  =>  \cdots
sin  =>  \sin
```

还有特别重要的数集、向量、矩阵符号：

```text
RR  =>  \mathbb{R}
NN  =>   \mathbb{N}
txt  =>  \text{...}
xbar  =>  \bar{x}
xhat  =>  \hat{x}
xhvec  =>  \vec{x}
xhdot  =>  \dot{x}
Xbb  =>  \mathbb{X}
Xbs  =>  \boldsymbol{X}
Xbm  =>  \bm{X}
Xbf  =>  \mathbf{X}
Xsf  =>  \mathsf{X}
Xcal  =>  \mathcal{X}
Xfrak  =>  \mathfrak{X}
Xrm  =>  \mathrm{X}
```

## 输出为 PDF

我们在右侧预览栏邮件菜单, 选择 **在浏览器中打开**.



![img](https://pic2.zhimg.com/80/v2-268e98a57310dcc2899feeedf5b21a41_1440w.webp)



在浏览器中右键选择 **打印**.



![img](https://pic1.zhimg.com/80/v2-969bb5cd58fb4a32c5a2b20cf5814b4c_1440w.webp)



就能够 **输出为 PDF** 了.



![img](https://pic3.zhimg.com/80/v2-f4608a8872385ae97310a94b4a035846_1440w.webp)



## 类似 UltiSnips 的自动补全

也许你曾经看过这篇文章：

[机器之心：世界上最好的编辑器Vim：1700多页数学笔记是如何实时完成的](https://zhuanlan.zhihu.com/p/61036165)
于是你很想试一下, 然后就被 Vim 和 Latex 给劝退了。

但是实际上, VS Code 完全能够替代 Vim, Markdown 在记笔记方面也完全能够替代 Latex. 通过 VS Code 插件 HyperSnips for Math, 你就可以像用 UtliSnips 一样使用各种神奇的 Snippets.

插件安装: [HyperSnips for Math - Visual Studio Marketplace](https://link.zhihu.com/?target=https%3A//marketplace.visualstudio.com/items%3FitemName%3DOrangeX4.hsnips)



![img](https://pic4.zhimg.com/80/v2-9a8764494374e3cf95c76ce54cbda74b_1440w.webp)



安装完成后, 按下快捷键 `Ctrl + Shift + P`, 输入命令 `Open Snippets Directory`, 就可以打开一个文件夹. 在该文件夹新建一个文件 `markdown.hsnips`, 并将 [这个网址](https://link.zhihu.com/?target=https%3A//github.com/OrangeX4/OrangeX4-HyperSnips/blob/main/markdown.hsnips) 里面的内容输入进去, 保存, 就可以使用了.

例如, 你可以在数学环境中输入: `(1+2)/`, 它会自动变为 `\frac{1+2}{}`.

你也可以创建自己的 Snippets, 按照格式, 发挥想象来写就好!

先看个 **普通例子**:

```text
snippet RR "R" iAm
\mathbb{R}
endsnippet
```

这是一个在数学环境中自动展开的 Snippet, 它有三个标示符 `iAm`, 分别代表 "在词语内部也会触发", "自动展开" 和 "数学环境".

这个例子会在数学环境内, 自动将 `RR` 展开成为 `\mathbb{R}`, 代表 "实数".

再看个 **正则表达式** 的例子:

```text
snippet `((\d+)|(\d*)(\\)?([A-Za-z]+)((\^|_)(\{\d+\}|\d))*)/` "Fraction no ()" Am
\frac{``rv = m[1]``}{$1}$0
endsnippet
```

其中 `rv = m[1]` 是 JavaScript 代码, 表示将正则表达式的第一个组 `m[1]` 输出给 "返回值" `rv`, 然后输出出去.

这是一个在数学环境中自动展开的 Snippet, 它有两个标示符 'Am', 分别代表 '自动展开' 和 '数学环境'. 用处是:

```text
1/    --->    \frac{1}{}
```

相比于原来的 HyperSnips, 最大特点是, 它只会在数学环境 `$...$`, `$$...$$`, `\(...\)` 和 `\[...\]` 中自动展开!

**还有 `${VISUAL}` 语法:**

```text
snippet fr "frac" iAm
\\frac{${1:${VISUAL}}}{$2}
endsnippet
```

这个语法会保存最近选中的内容, 然后替换掉 `${VISUAL}` 部分.

要开启在 markdown 下的 **自动补全提示**, 请使用 `Shift + Ctrl + P` 然后输入 `open settings json` 打开配置文件, 然后加入以下部分:

```json
"[markdown]": {
    "editor.quickSuggestions": true
},
```

## VS Code 快捷键

**快捷键**是用 VS Code 记笔记的**精髓**之一, 每一个都**非常重要**!

请务必**认真记住**这些快捷键!!!

### 原生快捷键

1. **通用操作**

2. 1. `Ctrl + C`, 复制当前文本
   2. `Ctrl + V`, 粘贴当前文本
   3. `Ctrl + Z`, 撤销
   4. `Ctrl + Shift + Z`, 反撤销
   5. `Shift + Alt + F`, 整理代码
   6. `Ctrl + /`, 将当前行注释 / 反注释, **当多行文本被选中时**, 将多行文本注释



1. **光标操作**

2. 1. `Ctrl + ←` 将光标向左移动一个**单词**
   2. `Ctrl + →` 将光标向右移动一个**单词**
   3. `Ctrl + Alt + ↑`, 向上加入一个光标
   4. `Ctrl + Alt + ↓`, 向下加入一个光标
   5. `Ctrl + Alt + U`, 撤销上次光标操作



1. **界面移动**

2. 1. `Ctrl + ↑` 向上移动当前界面
   2. `Ctrl + →` 向下移动当前界面



1. **选中操作**

2. 1. `Shift + ←` 向左选中 / 反选中一个**字符****(重要)**
   2. `Shift + →` 向右选中 / 反选中一个**字符****(重要)**
   3. `Ctrl + Shift + ←` 向左选中 / 反选中一个**单词****(重要)**
   4. `Ctrl + Shift + →` 向右选中 / 反选中一个**单词****(重要)**
   5. `Ctrl + D`**当前有选中文本时**, 将下一个与其相同的文本加入选中 **(重要)**



1. **文本行操作**

2. 1. `Ctrl + C`**当前无选中文本时**, 复制当前行
   2. `Shift + Alt + ↑` 向上**复制**当前行, **当多行文本被选中时**, 向上复制多行 **(重要)**
   3. `Shift + Alt + ↓` 向下**复制**当前行, **当多行文本被选中时**, 向下复制多行 **(重要)**
   4. `Alt + ↑` 向上**移动**当前行, **当多行文本被选中时**, 将当前多行文本向上移动 **(重要)**
   5. `Alt + ↓` 向下**移动**当前行, **当多行文本被选中时**, 将当前多行文本向下移动 **(重要)**



### 插件增加的快捷键

1. **Markdown 语法**

2. 1. `Ctrl + B`**当前有选中文本时**, 将文本加粗
   2. `Ctrl + I`**当前有选中文本时**, 将文本变为斜体
   3. `Ctrl + M` 进入数学公式模式 (加入美元符)



1. **图片粘贴**

2. 1. `Ctrl + Alt + V` 粘贴剪贴板图片 (本地)
   2. `Ctrl + Alt + V` 粘贴剪贴板图片 (图床)



1. **光标操作**

2. 1. `Ctrl + Alt + U` 将多选光标变为单选



1. **选中操作**

2. 1. `Shift + Alt + ←` 向左**复制**当前选中文本 **(重要)**
   2. `Shift + Alt + →` 向右**复制**当前选中文本 **(重要)**
   3. `Alt + ←` 向左**移动**当前选中文本一个**字符****(重要)**
   4. `Alt + →` 向右**移动**当前选中文本一个**字符****(重要)**
   5. `Ctrl + Alt + ←` 向左**移动**当前选中文本一个**单词****(重要)**
   6. `Ctrl + Alt + →` 向右**移动**当前选中文本一个**单词****(重要)**



1. **计算器功能**

2. 1. `Ctrl + Shift + Alt + E` 计算当前选中表达式, **用等号连接**并输出
   2. `Ctrl + Shift + Alt + R` 计算当前选中表达式, 并**替换当前选中表达式**
   3. `Ctrl + Shift + Alt + D` 定义当前选中表达式, **无输出**



## 科学计算

使用我开发的一个插件 `Latex Markdown Calculator` , 可以很方便地在 VS Code 中用 Latex 公式语法进行科学计算。

即选中一段数学表达式, 按下一个快捷键就能帮你计算出结果, 一些简单的计算再也不用打开电脑自带的计算器和 Matlab~

因为是基于 Python Sympy 的, 所以现在它已经有很多强大的功能了。

比如说：符号运算, 求积分, 求微分, 基于矩阵的符号运算(如行列式, 点乘, 转置, 求逆等功能), 解方程...

快捷键为 `Shift + Ctrl + Alt + E`, 详细内容请查看插件的说明文档.



![img](https://pic4.zhimg.com/80/v2-59abfbec7f2ac3d8d0c435cfc1c8551f_1440w.webp)





![img](https://pic3.zhimg.com/80/v2-efebb5656c06fb94635f4cb82f82000e_1440w.webp)



## 云端存储

### 安装 Git

你可以前往 [官网](https://link.zhihu.com/?target=https%3A//git-scm.com/downloads) 下载 Git, 有 Windows 版本, 也有 Mac 版本和 Linux 版本.



![img](https://pic4.zhimg.com/80/v2-8a602441e83fc0189ae0e72808098f7f_1440w.webp)



如果你网速不佳, 也可以去 [腾讯软件中心](https://link.zhihu.com/?target=https%3A//pc.qq.com/detail/13/detail_22693.html) 下载.

安装过程中, 基本上一直点 `Next` 就好.



![img](https://pic3.zhimg.com/80/v2-34b7f438ee06c3e73733bc31288fa246_1440w.webp)



安装好了之后, 按下 `Win` 键, 输入 `cmd`, 回车, 便出现了命令行.

输入

```text
git
```

命令, 回车, 若输出如图显示, Git 就安装成功了.



![img](https://pic2.zhimg.com/80/v2-ad0cf1a51c73590fef6439bffbcbf859_1440w.webp)



### 版本控制

我们使用 Git 来实现版本控制, 或者是笔记保存效果.

**每次你更改了笔记, 在传到云端之前, 都要进行一次笔记保存 Commit.**



![img](https://pic4.zhimg.com/80/v2-4ba2ef6abc6c42bca770d7f6cb6d7b3b_1440w.webp)





![img](https://pic3.zhimg.com/80/v2-33f93621f386a3268826818c32fa2d86_1440w.webp)





![img](https://pic1.zhimg.com/80/v2-22533f0c8bcdbed49dff8ff9a3033c94_1440w.webp)



### 上传到 GitHub

GitHub 是世界上最大的代码托管平台, 你当然也可以把你的笔记托管在 GitHub 上.

你可以看我的这篇 [GitHub 简易指南](https://link.zhihu.com/?target=https%3A//orangex4.cool/post/github-tutorials-for-beginner/), 加深对 GitHub 的理解.

要上 GitHub, 你可能需要一点小技巧, 这我就不教你了.

不然你也可以选择国内的 Gitee 或者国内能访问的 GitLab.

看完这篇指南之后, 你大概就知道怎么把笔记托管到云端了, 而且, 完全免费噢.

(虽然可能麻烦了点)

### 上传云端

**如果你设置好了 GitHub**, 需要上传到云端了, 你可以 Git Push 上去.



![img](https://pic1.zhimg.com/80/v2-a2d66edb0b0aa77346c631c5da853d78_1440w.webp)



## 在线浏览

**如果你把你的笔记上传到了云端**, 你就可以**随时随地**地查看你的笔记, 并且可以很方便地**分享给别人**.

比如, 你要看我的笔记, 可以访问这个链接:

[https://notes.orangex4.cool/?git=gitlab](https://link.zhihu.com/?target=https%3A//notes.orangex4.cool/%3Fgit%3Dgitlab)

如果你把你的笔记上传到了 GitHub, 想要查看, 你可以用这个网址:

[https://notes.orangex4.cool/](https://link.zhihu.com/?target=https%3A//notes.orangex4.cool/)

并且仿照这个格式:

[https://notes.orangex4.cool/?git=github&github=typoverflow/note](https://link.zhihu.com/?target=https%3A//notes.orangex4.cool/%3Fgit%3Dgithub%26github%3Dtypoverflow/note)

大概格式是:

[https://notes.orangex4.cool/?git=github&github=](https://link.zhihu.com/?target=https%3A//notes.orangex4.cool/%3Fgit%3Dgithub%26github%3D)用户名/笔记仓库

你就有了这种效果的笔记!



![img](https://pic4.zhimg.com/80/v2-28ed5a7053e44ce56d5b833868bd3a97_1440w.webp)



## Markdown 进阶 (选看)

**Markdown Preview Enhanced** 提供了非常强大的功能, 你可以访问 [MPE 简介](https://link.zhihu.com/?target=https%3A//shd101wyy.github.io/markdown-preview-enhanced/%23/zh-cn/) 获取更多相关的信息.

例如说, 你可以:

### 自动目录

只需要使用语法

```text
[TOC]
```

就能自动生成目录.

### 画图

### 流程图



![img](https://pic3.zhimg.com/80/v2-d2a6caacfbf8ce0f00f1ee729184dda2_1440w.webp)



### 时序图



![img](https://pic4.zhimg.com/80/v2-b1d18378ba1422488aa744d58f47e2c3_1440w.webp)



### 其他

你可以自己访问 [MPE 简介](https://link.zhihu.com/?target=https%3A//shd101wyy.github.io/markdown-preview-enhanced/%23/zh-cn/) 获取更多相关的信息.

### 代码块

你可以在 Markdown 中运行 **Python**, **Javascript** 之类的代码!

甚至可以运行 **Latex**!



![img](https://pic3.zhimg.com/80/v2-0e90dd5b8bfbbba80ab3a0f3258c1f2e_1440w.webp)



详见 [Code Chunk](https://link.zhihu.com/?target=https%3A//shd101wyy.github.io/markdown-preview-enhanced/%23/zh-cn/code-chunk).

### 软件推荐

### Snipaste

超良心的截图软件, 而且可以**贴图到屏幕上**, 写作业神器!



![img](https://pic1.zhimg.com/80/v2-1739d9d5425d37c9f51386d06cc3fc54_1440w.webp)



### GeoGebra

[GeoGebra 官网](https://link.zhihu.com/?target=https%3A//www.geogebra.org/)

你可以很方便地画函数图像!



![img](https://pic2.zhimg.com/80/v2-10ae9e60b9c785e2e64d0a0d288f7095_1440w.webp)



### Drawio

超良心的免费画图软件, 你可以用它画**流程图**, **电路图**之类的各种图.

对齐功能超赞, 而且完全免费!

而且可以**不用下载, 在线使用!**

当然你要离线用也可以下离线版本, 甚至可以下载对应的 VS Code 插件!

[Drawio 官网](https://link.zhihu.com/?target=https%3A//app.diagrams.net/)



![img](https://pic1.zhimg.com/80/v2-64a0a19bcf554a16c454e7e799ac16b0_1440w.webp)



## 总结

暂时想到的就这些啦, 更多的内容后续再补充, 也欢迎给我提交意见~

顺便推荐一下我写的「计算机学生的第零课」系列文章。您可以通过下方链接查看完整目录。