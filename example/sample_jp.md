% KiTTy での数式表現
% Kray-G
% August 22, 2021

<param style="JArticleA4"/>
<style-info name="code.lineNumber" value="false"/>
<style-info name="code.box" value="BOX_NORMAL"/>

# 概要

KiTTy では美しい数式表現をサポートしています。
次の例をご覧ください。

```math
f(r) = \pi r^2
```

このような数式を簡単に挿入できます。

インラインで数式を使う場合は `$\\pi$` といった形で `$` で数式表現を囲むことで $\\pi$ と文章中に表現することができます。
この時、バックスラッシュを重ねる必要があることに注意してください。

また、上記例のように独立した行で数式を扱う際は、<backq3 /> に `math` を指定して以下のように記述します。

    ```math
    f(r) = \pi r^2
    ```

このように記述すると、独立した行に大きな形で数式を表現することができます。

実は KiTTy では内部に \\KaTeX を内蔵しています。
したがって、\\KaTeX で表現可能な数式は全て利用可能です。
数式を美しく表現できることで、表現力豊かな文章作成が可能です。

# 様々な数式のサンプル

ここでは有名な数式をいくつかご紹介しましょう。

## ピタゴラスの定理

直角三角形の斜辺の長さを $c$、他の2辺の長さを $a$、$b$ とすると、次の式が成り立ちます。

```math
a^2 + b^2 = c^2
```

非常に有名な公式で、
\\url[https://ja.wikipedia.org/wiki/%E3%83%94%E3%82%BF%E3%82%B4%E3%83%A9%E3%82%B9%E3%81%AE%E5%AE%9A%E7%90%86]{Wikipedia} を見ると非常に多くの証明方法があります。
これは次のように記述します。

```
a^2 + b^2 = c^2
```

## オイラーの等式

ネイピア数 $e$、虚数 $i$、円周率 $\\pi$ と有名な定数を含む、非常に美しい数式です。

```math
e^{i\pi} + 1 = 0
```

次のように記述します。

```
e^{i\pi} + 1 = 0
```

## オイラーの公式

微分方程式を解く際によく使う公式です。

```math
e^{i\theta} = \cos\theta + i \sin\theta
```

三角関数もサポートしています。
`$\\sin\\theta$、$\\cos\\theta$、$\\tan\\theta$` はそれぞれ $\\sin\\theta$、$\\cos\\theta$、$\\tan\\theta$ と表現されます。
$\\alpha$、$\\beta$、$\\gamma$ などのギリシャ文字は、頭文字を大文字にして `\Theta` とすると、$\\Theta$ といった形で大文字のギリシャ文字になります。
これは次のように記述します。

```
e^{i\theta} = \cos\theta + i \sin\theta
```

## 正規分布（ガウス分布）

平均を $\\mu$、分散を $\\sigma^2 \\gt 0$ とする正規分布とは、確率密度関数が次の形で与えられる確率分布のことを言います。

```math
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp{\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)}
```

統計学の分野における重要な数式です。
この数式はグラフで表すと綺麗な釣り鐘型の曲線になります。
$\\mu \\pm \\sigma$ が変曲点となるのが特徴です。
これは次のように記述します。

```
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp{\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)}
```

## ガウス積分

ガウス積分あるいはオイラー＝ポアソン積分です。

```math
\int_{-\infty}^{\infty} f(x) dx = \sqrt{\pi}
```

インテグラルなど数式として書きたくなる式です。
これが書きたいがゆえに \\LaTeX を使うイメージでしょうか（勝手なイメージ）。
これは次のように記述します。

```
\int_{-\infty}^{\infty} f(x) dx = \sqrt{\pi}
```

## 調和数（発散列）

n-番目の調和数とは 1 から n までの自然数の逆数和のことを言います。

```math
\frac{1}{1} + \frac{1}{2} + \frac{1}{3} + \dots = \displaystyle\sum_{i=1}^\infty \frac{1}{n}= \infty
```

不思議なことに、なぜか分数を極限まで足していくと発散します。
オイラーの等式もそうですが、数学のこういう不思議な性質を見て数学にハマっていく方も多いかと思います。
これは次のように記述します。

```
\frac{1}{1} + \frac{1}{2} + \frac{1}{3} + \dots
  = \displaystyle\sum_{i=1}^\infty \frac{1}{n}= \infty
```

## バーゼル問題

バーゼル問題とは級数の問題の一つで、平方数の逆数全ての和はいくつかという問題のことを言います。

```math
\frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2} + \dots
  = \displaystyle\sum_{i=1}^\infty \frac{1}{n^2}= \frac{\pi^2}{6}
```

調和数と似ていますが、なぜか分母を 2 乗にするだけで収束するようになります。
なぜでしょう。面白いですね。
これは次のように記述します。

```
\frac{1}{1^2} + \frac{1}{2^2} + \frac{1}{3^2} + \dots
  = \displaystyle\sum_{i=1}^\infty \frac{1}{n^2}= \frac{\pi^2}{6}
```

## 行列

行列を表現してみましょう。

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

先の調和数などでも使ったドットですが、行列を表す際にはこのようにドットを縦横に並べることもできます。
次のように記述します。

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
