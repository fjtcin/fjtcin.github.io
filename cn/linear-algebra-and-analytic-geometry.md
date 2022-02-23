---
layout: page
title: 陈发来线代听课笔记
---

# [陈发来线代](https://www.icourses.cn/sCourse/course_3066.html)听课笔记
{:.no_toc}

```text
《线性代数与解析几何》 第二版 陈发来、陈效群、李思敏、王新茂 高等教育出版社 2015/8/1
 I  S  B  N： 978-7-04-043312-8  定价：29.80
```

## 目录
{:.no_toc}

* .
{:toc}

## 1&emsp;向量与复数

### 1.1&emsp;向量的线性运算

#### 1.1.3&emsp;向量的共线与共面

知道向量的共线、共面关系的表示后，点的共线、共面关系也可以表示出来。**（不要搞混了。）**

三点 \\(A,B,C\\) 共线 \\(\iff \overrightarrow{OA}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}, \lambda'+\mu'=1, O\\) 是平面中任意一点。

> Proof：\\(\overrightarrow{AB}\\) are parallel to \\(\overrightarrow{AC}\\)
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

特别地，当 \\(A\\) 是三角形重心时，\\(\overrightarrow{OA}=\frac{1}{3}\overrightarrow{OB}+\frac{1}{3}\overrightarrow{OC}+\frac{1}{3}\overrightarrow{OD}\\)

当 \\(A\\) 是三角形内心时，\\(\overrightarrow{OA}=\frac{\lvert CD \rvert\overrightarrow{OB}+\lvert DB \rvert\overrightarrow{OC}+\lvert BC \rvert\overrightarrow{OD}}{\lvert BC \rvert+\lvert CD \rvert+\lvert DB \rvert}\\)

当 \\(O, A\\) 重合时，\\(\bm{0}=\lambda'\overrightarrow{OB}+\mu'\overrightarrow{OC}+\nu'\overrightarrow{OD}\\)

当 \\(O\\) 在三角形的边上时，退化为定比分点之情形。

当 \\(O\\) 在三角形的顶点上时，退化为 \\(\overrightarrow{OB}=\overrightarrow{OB}\\)

---

```text
Febuary, 2022; Suzhou, China;
Dedicated to her with love.

Please feel free to add a comment if you witness ANY error.
Last modified on 2/23/2022, UPDATING...
```
