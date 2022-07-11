---
layout: post
title: An ODE Problem
latex: \(xy'+y=axy^2\ln x\)
categories: math
---

# $$xy'+y=axy^2\ln x$$

## Method 1: Solving the Bernoulli's Equation

Divide both sides by $$x$$, and we get the Bernoulli's equation:

$$
\frac{dy}{dx}+\frac{1}{x}y=a\ln(x)y^2
$$

Divide both sides by $$y^2$$:

$$
\frac{1}{y^2}\frac{dy}{dx}+\frac{1}{xy}=a\ln x
$$

Let $$u=\frac{1}{y}$$, and we get a first-order linear ODE:

$$
\frac{du}{dx}-\frac{1}{x}u=-a\ln x
$$

(Variation of Parameters) Let $$u(x)=C(x)e^{-\int-\frac{1}{x}\,dx}=xC(x)$$:

$$
x\frac{dC(x)}{dx}=-a\ln x
$$

Hence,

$$
\frac{dC(x)}{dx}=-\frac{a\ln x}{x}
$$

Integrate both sides with respect to $$x$$ and evaluate the integrals:

$$
\frac{u}{x}=-\frac{1}{2}a\ln^2x+C
$$

Substitute $$u=\frac{1}{y}$$:

$$
y=\frac{2}{Cx-ax\ln^2x}
$$

## Method 2: Oberservation

Multiply both sides by $$dx$$:

$$
x\,dy+y\,dx=axy^2\ln x\,dx
$$

Divide both sides by $$x^2y^2$$:

$$
\frac{x\,dy+y\,dx}{x^2y^2}=\frac{a\ln x}{x}\,dx
$$

Hence,

$$
-d\left(\frac{1}{xy}\right)=\frac{a}{2}\,d\left(\ln^2x\right)
$$

Integrate both sides:

$$
\frac{1}{xy}=-\frac{a}{2}\ln^2x+C
$$

Solve for $$y$$:

$$
y=\frac{2}{Cx-ax\ln^2x}
$$

## Method 3: Integrating Factor

Multiply both sides by $$dx$$:

$$
\left(y-axy^2\ln^2x\right)\,dx+x\,dy=0
$$

It admits $$\mu(x)=\frac{1}{x^2y^2}$$ as an integrating factor:

$$
\frac{y-axy^2\ln^2x}{x^2y^2}\,dx+\frac{1}{xy^2}\,dy=0
$$

Observe that:

$$
\frac{y-axy^2\ln^2x}{x^2y^2}\,dx+\frac{1}{xy^2}\,dy=d\left(\frac{1}{xy}+\frac{a}{2}\ln^2x\right)
$$

Hence,

$$
\frac{1}{xy}+\frac{a}{2}\ln^2x=C
$$

Solve for $$y$$:

$$
y=\frac{2}{Cx-ax\ln^2x}
$$

```text
May, 2022; Hefei, China.
Dedicated to Yang.

Please feel free to add a comment if you witness ANY error.
Last modified on 5/9/2022.
```
