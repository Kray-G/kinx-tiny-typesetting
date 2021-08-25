% Mathematical Expressions in KiTTy
% Kray-G
% August 22, 2021

<param style="ArticleA4"/>
<style-info name="code.lineNumber" value="false"/>
<style-info name="code.box" value="BOX_NORMAL"/>

# Overview

KiTTy supports a beautiful representation of mathematical expressions.
Look at the example below.

```math
f(r) = \pi r^2
```

You can easily insert mathematical expressions like this into your document.

If you use it inline, use `$\\pi$` as wrapping around an expression by `$` and you can see $\\pi$ in the sentense.
Note that a backslash should be double in this case.

If you want to use it in the independent line, use <backq3 /> with `math` as below.

    ```math
    f(r) = \pi r^2
    ```

By this manner, you can see mathematical expressions as a big size in the independent line.

In fact, KiTTy has \\KaTeX inside.
Thereby, all of mathematical expressions that \\KaTeX can present is available.
The ability to present a beautiful mathematical expression allows for expressive writing.

# Various Samples of Mathematical Expressions

Let\\apos{}s introduce some of famous expressions and fomulas.

## Pythagorean Theorem

When the length of the hypotenuse of a right triangle is $c$ and the length of other sides are $a$ and $b$, then the following equation holds.

```math
a^2 + b^2 = c^2
```

This is very famous formula, and looking at \\url[https://en.wikipedia.org/wiki/Pythagorean_theorem]{Wikipedia}, there are so many ways to prove it.
You can write it as below.

```
a^2 + b^2 = c^2
```

## Euler\\apos{}s Identity

It is a very beautiful mathematical expression containing the Napier number $e$, the imaginary number $i$, pi $\\pi$ and the famous constant.

```math
e^{i\pi} + 1 = 0
```

You can write it as below.

```
e^{i\pi} + 1 = 0
```

## Euler\\apos{}s Formula

This is a formula that is often used when solving differential equations.

```math
e^{i\theta} = \cos\theta + i \sin\theta
```

Trigonometric functions are also supported.
If you write `$\\sin\\theta$`, `$\\cos\\theta$`, `$\\tan\\theta$`, it will be represented as $\\sin\\theta$, $\\cos\\theta$, $\\tan\\theta$.
Regarding Greek letters such as $\\alpha$, $\\beta$, $\\gamma$, etc., capitalized Greek letters are shown like $\\Theta$ if making the first letter capitalized such as `\Theta`.
You can write it as below.

```
e^{i\theta} = \cos\theta + i \sin\theta
```

## Normal Distribution (Gauss Distribution)

A normal distribution with $\\mu$ as the mean and $\\sigma^2\\gt 0$ as the variance is a probability distribution which probability density function is given by the following formula.

```math
f(x) = \frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}
```

This is an important formula in the field of statistics.
This equation is gives a beautiful bell-shaped curve on the graph.
It is characterized that $\\mu \\pm \\sigma$ is an inflection point.

```
f(x) = \frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}
```

## Gaussian Integral

The Gaussian integral, or the Euler–Poisson integral.

```math
\int_{-\infty}^{\infty} f(x) dx = \sqrt{\pi}
```

An integral symbol, it is what you want to write as a mathematical expression.
I believe that is why we use \\LaTeX (just my guess).
You can write it as follows.

```
\int_{-\infty}^{\infty} f(x) dx = \sqrt{\pi}
```

## Harmonic Number

The n-th harmonic number is the sum of the reciprocals of the first n natural numbers:

```math
\frac{1}{1} + \frac{1}{2} + \frac{1}{3} + \dots = \displaystyle\sum_{i=1}^\infty \frac{1}{n}= \infty
```

Strangely enough, when you add fractions to the limit, they diverge.
Like Euler\\apos{}s Identity, many people might be into mathematics by seeing such mysterious properties.

```
\frac{1}{1} + \frac{1}{2} + \frac{1}{3} + \dots
  = \displaystyle\sum_{i=1}^\infty \frac{1}{n}= \infty
```

## Basel Problem

The Basel problem is one of the problems of series, which is how many is the sum of all the reciprocals of a square number.

```math
\frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2} + \dots
  = \displaystyle\sum_{i=1}^\infty \frac{1}{n^2}= \frac{\pi^2}{6}
```

It is similar to the harmonic numbers, but for some reason it converges just by making the denominator a square numer.
I wonder why. It is interesting.
It can be written as follows.

```
\frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2} + \dots
  = \displaystyle\sum_{i=1}^\infty \frac{1}{n^2}= \frac{\pi^2}{6}
```

## Matrix

Let\\apos{}s express a Matrix.

```math
A =
    \left(
    \begin{array}{cccc} 
        a_{11} & a_{12} & \ldots & a_{1n} \\ 
        a_{21} & a_{22} & \ldots & a_{2n} \\
        \vdots & \vdots & \ddots & \vdots \\
        a_{m1} & a_{m2} & \ldots & a_{mn} 
    \end{array}
    \right)
```

The dots used in the previous harmonic numbers, etc., can also be arranged horizontally and vertically like this to represent a matrix.
It can be written as follows

```
A =
    \left(
    \begin{array}{cccc} 
        a_{11} & a_{12} & \ldots & a_{1n} \\ 
        a_{21} & a_{22} & \ldots & a_{2n} \\
        \vdots & \vdots & \ddots & \vdots \\
        a_{m1} & a_{m2} & \ldots & a_{mn} 
    \end{array}
    \right)
```
