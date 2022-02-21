---
layout: page
---

# [陈发来线代](https://www.icourses.cn/sCourse/course_3066.html)听课笔记
{:.no_toc}

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

<script type="text/tikz">
\definecolor{ududff}{rgb}{0.30196078431372547,0.30196078431372547,1}
\begin{tikzpicture}[scale=1]
\clip(-8.92,-3.04) rectangle (4.92,2.48);
\draw [line width=2pt,domain=-3.92:3.92] plot(\x,{(-0.4528--2.8*\x)/2.64});
\begin{scriptsize}
\draw [fill=ududff] (-1.46,-1.72) circle (2.5pt);
\draw[color=ududff] (-1.3,-1.29) node {$A$};
\draw [fill=ududff] (1.18,1.08) circle (2.5pt);
\draw[color=ududff] (1.34,1.51) node {$B$};
\draw[color=black] (3.84,4.29) node {$f$};
\end{scriptsize}
\end{tikzpicture}
</script>

---

```text
Febuary, 2022; Suzhou, China;
Dedicated to her with love.

Please feel free to add a comment if you witness ANY error.
Last modified on 2/9/2022, UPDATING...
```
