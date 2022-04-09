---
layout: post
title: In Reply To A Projection Problem
categories: zhihu
---

# In Reply To A Projection Problem

[直线在平面上的摄影直线的求法（点法式）](https://www.zhihu.com/question/54139298/answer/2372811421)

[直线在平面上的摄影直线的求法（隐式）](https://www.zhihu.com/question/54139298/answer/1141428282)

[点到平面的摄影与到直线的摄影](https://www.zhihu.com/question/301830492/answer/2122446563)

求直线
$$
\left\{\begin{matrix}
2x-4y+z=0\\
3x-y-2z-9=0
\end{matrix}\right.
$$
在平面 $$4x-y+z=1$$ 上的投影直线的方程。

解：联立3个方程得平面与直线的交点为 $$\left(\frac{12}{13},-\frac{11}{39},-\frac{116}{39}\right)$$

平面的法向量 $$\bm{n}=\left(4,-1,1\right)$$，直线的方向向量 $$\bm{u}=\left(2,-4,1\right)\times\left(3,-1,-2\right)=\left(9,7,10\right)$$

则投影直线的方向向量 $$\bm{v}=-\left(\bm{u}\times\bm{n}\right)\times\bm{n}=\lvert\bm{n}\rvert^2\bm{u}-\left(\bm{u}\cdot\bm{n}\right)\bm{n}=\left(6,165,141\right)$$

故直线方程为 $$\frac{x-\frac{12}{13}}{6}=\frac{y+\frac{11}{39}}{165}=\frac{z+\frac{116}{39}}{141}$$

以上的方法比较适用于给定直线点法式的情况。但在本题中，给定的是直线的隐式方程，运用[有轴平面束的方法](https://www.zhihu.com/question/54139298/answer/1141428282)更简便，算得 $$\lambda=-\frac{13}{11}$$，直线的隐式方程为

$$
\left\{\begin{matrix}
-17x-31y+37z+117=0\\
4x-y+z-1=0
\end{matrix}\right.
$$

---

```text
March, 2022; Hefei, China;

Please feel free to add a comment if you witness ANY error.
Last modified on 3/8/2022
```
