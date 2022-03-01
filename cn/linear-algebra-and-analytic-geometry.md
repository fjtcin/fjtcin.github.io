---
layout: page
title: 陈发来线代听课笔记
---

# [陈发来线代](https://www.icourses.cn/sCourse/course_3066.html)听课笔记
{:.no_toc}

```text
《线性代数与解析几何》 第二版 陈发来、陈效群、李思敏、王新茂 高等教育出版社 2015/8/1
 I  S  B  N： 978-7-04-043312-8  定价：29.80

视频中的错误：
第二章-第1课 —— 直线与平面方程 —— 22:22：implicit 拼错。
```

各个教授在授课时都会讲些教材上没有的内容，即所谓的“拓展内容”。本文提取了陈发来教授的所有拓展内容，读者应结合书本阅读。[陈发来教授](http://staff.ustc.edu.cn/~chenfl/)是[中国科学技术大学](https://ustc.edu.cn/)的名教师，在[评课社区](https://icourse.club/course/5479/)好评如潮。读者在读完教材和本文后就完全掌握了课堂的所有知识，无需再看视频，节约了时间。

## 目录
{:.no_toc}

* .
{:toc}

## 1&emsp;向量与复数

### 1.1&emsp;向量的线性运算

#### 1.1.3&emsp;向量的共线与共面

知道向量的共线、共面关系的表示后，点的共线、共面关系也可以表示出来。**（不要搞混了。）**

三点 \\(A,B,C\\) 共线 \\(\iff \overrightarrow{OA}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}, \lambda'+\mu'=1, O\\) 是平面中任意一点。

> Proof: \\(\overrightarrow{AB}\\) are parallel to \\(\overrightarrow{AC}\\)
>
> \\(\iff\\) there exists \\(\lambda, \mu\\) (not all 0) such that \\(\lambda\overrightarrow{AB}+\mu\overrightarrow{AC}=0\\)
>
> \\(\iff \lambda\left(\overrightarrow{OB}-\overrightarrow{OA}\right)+\mu\\left(\overrightarrow{OC}-\overrightarrow{OA}\right)=0\\)
>
> \\(\iff \left(\lambda+\mu\right)\overrightarrow{OA}=\lambda\overrightarrow{OB}+\mu\overrightarrow{OC}\\)
>
> If \\(\lambda+\mu=0\\), then \\(\overrightarrow{OB}=\overrightarrow{OC}\\) for arbitrary point \\(O\\), which means \\(B\\) and \\(C\\) are the same points. That is not true, so \\(\lambda+\mu\neq 0\\) and we divide it from both sides.
>
> \\(\iff \overrightarrow{OA}=\frac{\lambda}{\lambda+\mu}\overrightarrow{OB}+\frac{\mu}{\lambda+\mu}\overrightarrow{OC}\\)
>
> Denote \\(\lambda'=\frac{\lambda}{\lambda+\mu}\\) and \\(\mu'=\frac{\mu}{\lambda+\mu}\\), and we get
>
> \\(\iff \overrightarrow{OA}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}, \lambda'+\mu'=1\\)

四点 \\(A,B,C,D\\) 共面 \\(\iff \overrightarrow{OA}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}+\nu'\overrightarrow{OD}, \lambda'+\mu'+\nu'=1, O\\) 是空间中任意一点。

以上内容实际上是**例 1.1.2** 的直接推论。同时，它们也有深刻的几何意义：

<div align="center">
<script type="text/tikz">
\definecolor{xdxdff}{rgb}{0.49019607843137253,0.49019607843137253,1}
\definecolor{ududff}{rgb}{0.30196078431372547,0.30196078431372547,1}
\begin{tikzpicture}[scale=1]
\clip(-3,-4.5) rectangle (11,1.4);
\draw [line width=1pt] (3.96,0.96)-- (-0.06,-4.12);
\draw [line width=1pt] (3.96,0.96)-- (7.22,-4.08);
\draw [line width=1pt,domain=-8.92:16.68] plot(\x,{(-29.9912--0.04*\x)/7.28});
\draw [line width=1pt] (3.96,0.96)-- (3.100124377358491,-4.1026366792452835);
\begin{scriptsize}
\draw [fill=ududff] (3.96,0.96) circle (2.5pt);
\draw[color=ududff] (4.12,1.3) node {$O$};
\draw [fill=ududff] (-0.06,-4.12) circle (2.5pt);
\draw[color=ududff] (-0.34,-3.57) node {$B$};
\draw [fill=ududff] (7.22,-4.08) circle (2.5pt);
\draw[color=ududff] (7.38,-3.49) node {$C$};
\draw [fill=xdxdff] (3.100124377358491,-4.1026366792452835) circle (2.5pt);
\draw[color=xdxdff] (3.56,-3.59) node {$A$};
\end{scriptsize}
\end{tikzpicture}
</script>
\\(A\\) 是直线 \\(BC\\) 上一点（称作定比分点）。\\(O\\) 是平面上任意一点。
</div>

$$
\overrightarrow{OA}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}\\
\lambda'+\mu'=1\\
\lambda'=\overline{AC}\bigg/\overline{BC}\\
\text{note that }\overline{AC}=x_C-x_A\text{ (the directed line segment), so }\overline{BA}+\overline{AC}\equiv \overline{BC}
$$

<div align="center">
<div style="display:inline-block;">
<script type="text/tikz">
\definecolor{ffqqtt}{rgb}{1,0,0.2}
\definecolor{qqccqq}{rgb}{0,0.8,0}
\definecolor{zzttqq}{rgb}{0.6,0.2,0}
\definecolor{xdxdff}{rgb}{0.49019607843137253,0.49019607843137253,1}
\definecolor{ududff}{rgb}{0.30196078431372547,0.30196078431372547,1}
\begin{tikzpicture}[scale=0.75]
\fill[line width=2pt,color=zzttqq,fill=zzttqq,fill opacity=0.10000000149011612] (0.32,4.78) -- (-4.06,-1.8) -- (5.3,-1.76) -- cycle;
\fill[line width=2pt,color=qqccqq,fill=qqccqq,fill opacity=0.1] (0.32,4.78) -- (0.54,0.92) -- (-4.06,-1.8) -- cycle;
\fill[line width=2pt,color=ffqqtt,fill=ffqqtt,fill opacity=0.1] (0.32,4.78) -- (0.54,0.92) -- (5.3,-1.76) -- cycle;
\draw [line width=2pt,color=zzttqq] (0.32,4.78)-- (-4.06,-1.8);
\draw [line width=2pt,color=zzttqq] (-4.06,-1.8)-- (5.3,-1.76);
\draw [line width=2pt,color=zzttqq] (5.3,-1.76)-- (0.32,4.78);
\draw [line width=2pt,color=qqccqq] (0.32,4.78)-- (0.54,0.92);
\draw [line width=2pt,color=qqccqq] (0.54,0.92)-- (-4.06,-1.8);
\draw [line width=2pt,color=qqccqq] (-4.06,-1.8)-- (0.32,4.78);
\draw [line width=2pt,color=ffqqtt] (0.32,4.78)-- (0.54,0.92);
\draw [line width=2pt,color=ffqqtt] (0.54,0.92)-- (5.3,-1.76);
\draw [line width=2pt,color=ffqqtt] (5.3,-1.76)-- (0.32,4.78);
\begin{scriptsize}
\draw [fill=ududff] (0.32,4.78) circle (2.5pt);
\draw[color=ududff] (0.56,5) node {$B$};
\draw [fill=ududff] (-4.06,-1.8) circle (2.5pt);
\draw[color=ududff] (-4.4,-1.31) node {$C$};
\draw [fill=ududff] (5.3,-1.76) circle (2.5pt);
\draw[color=ududff] (5.52,-1.25) node {$D$};
\draw [fill=xdxdff] (0.54,0.92) circle (2.5pt);
\draw[color=xdxdff] (0.94,1.35) node {$A$};
\end{scriptsize}
\end{tikzpicture}
</script>
</div>
<div style="display:inline-block;">
<script type="text/tikz">
\definecolor{ffqqtt}{rgb}{1,0,0.2}
\definecolor{qqccqq}{rgb}{0,0.8,0}
\definecolor{zzttqq}{rgb}{0.6,0.2,0}
\definecolor{xdxdff}{rgb}{0.49019607843137253,0.49019607843137253,1}
\definecolor{ududff}{rgb}{0.30196078431372547,0.30196078431372547,1}
\begin{tikzpicture}[scale=0.75]
\fill[line width=2pt,color=zzttqq,fill=zzttqq,fill opacity=0.10000000149011612] (0.32,4.78) -- (-4.06,-1.8) -- (5.3,-1.76) -- cycle;
\fill[line width=2pt,color=qqccqq,fill=qqccqq,fill opacity=0.1] (0.32,4.78) -- (-4.98,3.06) -- (-4.06,-1.8) -- cycle;
\fill[line width=2pt,color=ffqqtt,fill=ffqqtt,fill opacity=0.1] (0.32,4.78) -- (-4.98,3.06) -- (5.3,-1.76) -- cycle;
\draw [line width=2pt,color=zzttqq] (0.32,4.78)-- (-4.06,-1.8);
\draw [line width=2pt,color=zzttqq] (-4.06,-1.8)-- (5.3,-1.76);
\draw [line width=2pt,color=zzttqq] (5.3,-1.76)-- (0.32,4.78);
\draw [line width=2pt,color=qqccqq] (0.32,4.78)-- (-4.98,3.06);
\draw [line width=2pt,color=qqccqq] (-4.98,3.06)-- (-4.06,-1.8);
\draw [line width=2pt,color=qqccqq] (-4.06,-1.8)-- (0.32,4.78);
\draw [line width=2pt,color=ffqqtt] (0.32,4.78)-- (-4.98,3.06);
\draw [line width=2pt,color=ffqqtt] (-4.98,3.06)-- (5.3,-1.76);
\draw [line width=2pt,color=ffqqtt] (5.3,-1.76)-- (0.32,4.78);
\begin{scriptsize}
\draw [fill=ududff] (0.32,4.78) circle (2.5pt);
\draw[color=ududff] (0.56,5) node {$B$};
\draw [fill=ududff] (-4.06,-1.8) circle (2.5pt);
\draw[color=ududff] (-4.4,-1.6) node {$C$};
\draw [fill=ududff] (5.3,-1.76) circle (2.5pt);
\draw[color=ududff] (5.52,-1.5) node {$D$};
\draw [fill=xdxdff] (-4.98,3.06) circle (2.5pt);
\draw[color=xdxdff] (-4.86,3.5) node {$A$};
\end{scriptsize}
\end{tikzpicture}
</script>
</div>
\\(A\\) 是平面 \\(BCD\\) 上一点。\\(O\\) 是空间中任意一点。
</div>

$$
\overrightarrow{OA}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}+\nu'\overrightarrow{OD}\\
\lambda'+\mu'+\nu'=1\\
\lambda'=A\left(\triangle ACD\right)\bigg/A\left(\triangle BCD\right)\\
\text{note that the area can be negative here, so }A\left(\triangle ABC\right)+A\left(\triangle ACD\right)+A\left(\triangle ABD\right)\equiv A\left(\triangle BCD\right)
$$

> 证明：留做习题。

我们将 \\(\lambda', \mu', \nu'\\) 称为 \\(A\\) 关于 \\(\triangle BCD\\) 的面积坐标。看上去这个坐标有3个分量，实际上独立的只有2个，因为 \\(\lambda'+\mu'+\nu'=1\\)

特别地，当 \\(A\\) 是三角形重心时，\\(\overrightarrow{OA}=\frac{1}{3}\overrightarrow{OB}+\frac{1}{3}\overrightarrow{OC}+\frac{1}{3}\overrightarrow{OD}\\)

当 \\(A\\) 是三角形内心时，\\(\overrightarrow{OA}=\frac{\lvert CD\rvert\overrightarrow{OB}+\lvert DB\rvert\overrightarrow{OC}+\lvert BC\rvert\overrightarrow{OD}}{\lvert BC\rvert+\lvert CD\rvert+\lvert DB\rvert}\\)

当 \\(O, A\\) 重合时，\\(\bm{0}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}+\nu'\overrightarrow{OD}\\)

当 \\(O\\) 在三角形的边上时，退化为定比分点之情形。

当 \\(O\\) 在三角形的顶点上时，退化为 \\(\overrightarrow{OB}=\overrightarrow{OB}\\)

---

重心定理：三条中线交于一点。

> 证明：由**例 1.1.3** 知，\\(BE\\) 与 \\(AD\\) 的交点 \\(G\\) 满足 \\(\overrightarrow{AG}=\frac{2}{3}\overrightarrow{AD}\\)
>
> 同理，另一条中线与 \\(AD\\) 的交点 \\(G'\\) 满足 \\(\overrightarrow{AG'}=\frac{2}{3}\overrightarrow{AD}\\)
>
> 故 \\(G\\) 与 \\(G'\\) 是同一点。

### 1.4&emsp;向量的向量积

#### 1.4.1&emsp;向量积的定义与性质

（直角三棱锥的斜面面积的平方是其他三个面面积的平方和）在直角三棱锥 \\(O-ABC\\) 中，\\(A^2\left(\triangle ABC\right)=A^2\left(\triangle OAB\right)+A^2\left(\triangle OBC\right)+A^2\left(\triangle OCA\right)\\)

> 证明：记 \\(\bm{a}=\overrightarrow{OA}, \bm{b}=\overrightarrow{OB}, \bm{c}=\overrightarrow{OC}, a=\lvert\bm{a}\rvert, b=\lvert\bm{b}\rvert, c=\lvert\bm{c}\rvert\\)
>
> 则 \\(\overrightarrow{AB}=\bm{b}-\bm{a}, \overrightarrow{AC}=\bm{c}-\bm{a}, A\left(\triangle OAB\right)=\frac{1}{2}ab, A\left(\triangle OBC\right)=\frac{1}{2}bc, A\left(\triangle OCA\right)=\frac{1}{2}ac\\)
>
> \\(A^2\left(\triangle ABC\right)=\lvert\frac{1}{2}\left(\bm{b}\times\bm{c}-\bm{b}\times\bm{a}-\bm{a}\times\bm{c}\right)\rvert^2\\)
>
> 由于 \\(\bm{a}, \bm{b}, \bm{c}\\) 两两垂直，于是 \\(\bm{b}\times\bm{c}, \bm{b}\times\bm{a}, \bm{a}\times\bm{c}\\) 两两垂直，所以
>
> \\(A^2\left(\triangle ABC\right)=\frac{1}{4}\left(\lvert\bm{b}\times\bm{c}\rvert^2+\lvert\bm{b}\times\bm{a}\rvert^2+\lvert\bm{a}\times\bm{c}\rvert^2\right)=\frac{1}{4}\left(b^2c^2+b^2a^2+a^2c^2\right)\\)
>
> \\(=A^2\left(\triangle OAB\right)+A^2\left(\triangle OBC\right)+A^2\left(\triangle OCA\right)\\)

#### 1.4.2&emsp;直角坐标系下向量积的计算

三角形的三个顶点 \\(A\left(x_1, y_1, z_1\right), B\left(x_2, y_2, z_2\right), C\left(x_3, y_3, z_3\right)\\)，则 \\(A\left(\triangle ABC\right)=\frac{1}{2}\lvert\overrightarrow{AB}\times\overrightarrow{AC}\rvert\\)

特别地，当 \\(A=\left(x_1, y_1\right), B=\left(x_2, y_2\right), C=\left(x_3, y_3\right)\\) 时，

$$
A\left(\triangle ABC\right)
=\frac{1}{2}\left\lvert\begin{vmatrix}
\bm{i} & \bm{j} & \bm{k}\\
x_2-x_1 & y_2-y_1 & 0\\
x_3-x_1 & y_3-y_1 & 0
\end{vmatrix}\right\rvert
=\frac{1}{2}\left\lvert\begin{vmatrix}
x_2-x_1 & y_2-y_1\\
x_3-x_1 & y_3-y_1
\end{vmatrix}\right\rvert
=\frac{1}{2}\left\lvert\begin{vmatrix}
x_1 & x_2 & x_3\\
y_1 & y_2 & y_3\\
1 & 1 & 1
\end{vmatrix}\right\rvert
$$

同样地，四面体的四个顶点 \\(A\left(x_1, y_1, z_1\right), B\left(x_2, y_2, z_2\right), C\left(x_3, y_3, z_3\right), D\left(x_4, y_4, z_4\right)\\)，有

$$
V\left(ABCD\right)=\frac{1}{6}\left\lvert\begin{vmatrix}
x_1 & x_2 & x_3 & x_4\\
y_1 & y_2 & y_3 & y_4\\
z_1 & z_2 & z_3 & z_4\\
1 & 1 & 1 & 1
\end{vmatrix}\right\rvert
$$

**此处特别注意行列式中元素的顺序。**

### 1.5&emsp;向量的混合积

#### 1.5.1&emsp;混合积的定义

设不共面向量 \\(\bm{a}, \bm{b}, \bm{c}\\)，求 \\(\bm{x}\\) 满足 \\(\bm{a}\cdot\bm{x}=f, \bm{b}\cdot\bm{x}=g, \bm{c}\cdot\bm{x}=h\\)，其中 \\(f, g, h\\) 是给定的实数。

解：设 \\(\bm{x}=\lambda\bm{a}+\mu\bm{b}+\nu\bm{c}\\)，代入3个条件式得3个方程，解出 \\(\lambda, \mu, \nu\\) 即可。

上面的方法是最经典的方法，但极其难以计算。

注意到 [\\(\rm{a}, \rm{b}, \rm{c}\\) 共面等价于 \\(\rm{a}\times\rm{b}, \rm{b}\times\rm{c}, \rm{c}\times\rm{a}\\) 共面](https://www.zhihu.com/question/450742288/answer/2362517022)，故设 \\(\bm{x}=\lambda\bm{a}\times\bm{b}+\mu\bm{b}\times\bm{c}+\nu\bm{c}\times\bm{a}\\)，则

$$
\bm{a}\cdot\bm{x}=\mu\bm{a}\cdot\bm{b}\times\bm{c}=f\implies\mu=\frac{f}{\bm{a}\cdot\bm{b}\times\bm{c}}
$$

### 1.7&emsp;复数

#### 1.7.2&emsp;复数的几何表示

n倍角公式：利用 \\(\cos n\theta+i\sin n\theta=\left(\cos\theta+i\sin\theta\right)^n\\)

## 2&emsp;空间解析几何

### 2.1&emsp;直线与平面

#### 2.1.2&emsp;平面的方程

parametric equation: \\(\overrightarrow{OP}=\overrightarrow{OA}+s\overrightarrow{AB}+t\overrightarrow{AC}\\), non-unique

implicit equation (no parameters): \\(Ax+By+Cz+D=0\\), unique

**例 2.1.4** 已知三点，若求的是隐式方程，则可直接设 \\(\pi: Ax+By+Cz+D=0\\)，代入三点坐标解除一组 \\(A,B,C,D\\) 即可。

#### 2.1.5&emsp;两直线的位置关系

\\(A,B,\bm{u},\bm{v}\\) 分别是两直线上的点与方向向量，*公垂线 \\(\overrightarrow{CD}\\) 为 \\(\overrightarrow{AB}\\) 在 \\(\bm{u}\times\bm{v}\\) 方向上的投影*。

$$
\lvert\overrightarrow{CD}\rvert=\frac{\lvert\bm{u}\times\bm{v}\cdot\overrightarrow{AB}\rvert}{\lvert\bm{u}\times\bm{v}\rvert}
$$

所谓 *\\(\overrightarrow{AB}\\) 在 \\(\bm{u}\times\bm{v}\\) 方向上的投影*是指，在图 2.6 中，

$$
\frac{\lvert\bm{u}\times\bm{v}\cdot\overrightarrow{AB}\rvert}{\lvert\bm{u}\times\bm{v}\rvert}=\frac{\lvert\bm{u}\times\bm{v}\cdot(\overrightarrow{AC}+\overrightarrow{CD}+\overrightarrow{DB})\rvert}{\lvert\bm{u}\times\bm{v}\rvert}=\frac{\lvert\bm{u}\times\bm{v}\cdot\overrightarrow{CD}\rvert}{\lvert\bm{u}\times\bm{v}\rvert}=\lvert\overrightarrow{CD}\rvert
$$

### 2.2&emsp;空间曲线与曲面

建立空间曲面方程的方法：用向量来表示几何关系，再坐标化即可。

书上指出了给定准线参数方程时各曲面的方程。拓展内容是，我们在准线方程是隐式的情况下写出曲面满足的方程。
#### 2.2.2&emsp;柱面

准线方程

$$
\left\{\begin{matrix}
f\left(x,y,z\right)=0\\
g\left(x,y,z\right)=0
\end{matrix}\right.
$$

母线方向 \\(\bm{u}=\left(u_1,u_2,u_3\right)\\)

设 \\(P\left(x,y,z\right)\\) 曲面上任意一点，\\(Q\left(x_0,y_0,z_0\right)\\) 是其对应的准线上的点，则

$$
\left\{\begin{matrix}
x=x_0+su_1,y=y_0+su_2,z=z_0+su_3\\
f\left(x_0,y_0,z_0\right)=0\\
g\left(x_0,y_0,z_0\right)=0
\end{matrix}\right.
$$

即可得曲面方程为

$$
\left\{\begin{matrix}
f\left(x-su_1,y-su_2,z-su_3\right)=0\\
g\left(x-su_1,y-su_2,z-su_3\right)=0
\end{matrix}\right.
$$

以上内容可直接应用于 **例 2.2.5** 的求解。

#### 2.2.3&emsp;锥面

准线方程

$$
\left\{\begin{matrix}
f\left(x,y,z\right)=0\\
g\left(x,y,z\right)=0
\end{matrix}\right.
$$

顶点 \\(A\left(a_1,a_2,a_3\right)\\)

设 \\(P\left(x,y,z\right)\\) 曲面上任意一点，\\(Q\left(x_0,y_0,z_0\right)\\) 是其对应的准线上的点，故母线方向 \\(\bm{u}=\left(u_1,u_2,u_3\right)=\left(x_0-a_1,y_2-a_2,z_0-a_3\right)\\)

$$
\left\{\begin{matrix}
x=a_1+su_1,y=a_2+su_2,z=a_3+su_3\\
f\left(x_0,y_0,z_0\right)=0\\
g\left(x_0,y_0,z_0\right)=0
\end{matrix}\right.
$$

即可得曲面方程为

$$
\left\{\begin{matrix}
f\left(\frac{x-\left(1-s\right)a_1}{s},\frac{y-\left(1-s\right)a_2}{s},\frac{z-\left(1-s\right)a_3}{s}\right)=0\\
g\left(\frac{x-\left(1-s\right)a_1}{s},\frac{y-\left(1-s\right)a_2}{s},\frac{z-\left(1-s\right)a_3}{s}\right)=0
\end{matrix}\right.
$$

以上内容可直接应用于 **例 2.2.7** 的求解。

A cylindrical surface can be viewed as a limiting case of a conical surface whose apex is moved off to infinity in a particular direction. Indeed, in projective geometry a cylindrical surface is just a special case of a conical surface. [[1]](https://en.wikipedia.org/wiki/Conical_surface)

In projective geometry, a cylinder is simply a cone whose apex (vertex) lies on the plane at infinity. If the cone is a quadratic cone, the plane at infinity (which passes through the vertex) can intersect the cone at two real lines, a single real line (actually a coincident pair of lines), or only at the vertex. These cases give rise to the hyperbolic, parabolic or elliptic cylinders respectively.

This concept is useful when considering degenerate conics, which may include the cylindrical conics. [[2]](https://en.wikipedia.org/wiki/Cylinder#Projective_geometry)

## English-Chinese Technical Terms Table

读者可按 `Ctrl + F` 检索。

| English | 简体中文 |
| :---: | :---: |
| Quadric surface | 二次曲面 |
| Cylindrical surface (or degenerate quadric surface) | 柱面 |
| Apex | （锥面的）顶点 |
| Generatrix/generator/ruling | 母线 |
| Directrix | 准线 |
| Ruled surface | 直纹面 |
| Right circular cylinder | 圆柱面 |
| Elliptic cylinder | 椭圆柱面 |
| Hyperbolic cylinder | 双曲柱面 |
| Parabolic cylinder | 抛物柱面 |
| Ellipsoid | 椭球面 |
| One-sheet hyperboloid (or hyperbolic hyperboloid) | 单叶双曲面 |
| Two-sheet hyperboloid (or elliptic hyperboloid) | 双叶双曲面 |
| Conical quadric surface (or elliptic cone) | 二次锥面 |
| Hyperbolic paraboloid | 椭圆抛物面 |
| Hyperbolic paraboloid | 双曲抛物面（马鞍面） |
| Surface of revolution | 旋转曲面 |
| Diagonal | 对角线，对角线的 |

---

```text
Febuary, 2022; Suzhou&Hefei, China;
Dedicated to her with love.

Please feel free to add a comment if you witness ANY error.
Last modified on 2/28/2022, UPDATING...
```
