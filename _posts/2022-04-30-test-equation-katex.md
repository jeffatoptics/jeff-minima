---
layout: post
title: "test equation in katex"
categories: markdown
math: katex
author:
- jeffatoptics
---

$$
f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi
$$

> 📝 enable katex with front matter in current page:
> ```
> ---
> math: katex
> ---
> ```

1. math block:

    $$
    K(a,b) = \int \mathcal{D}x(t) \exp(2\pi i S[x]/\hbar)
    $$


1. math inline:

    this is inline function $f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$ and another inline function $ e = m c^2 $

    ```
    this is inline function $f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$ and another inline function $ e = m c^2 $
    ```
1.  some usages;
    inline is displayed: $$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$

    center is displayed:

    $$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$
    ```
    inline is displayed: $$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$

    center is displayed:

    $$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$
    ```
1. other equations for test:
    $$
    y=\frac{1}{2} \times \sqrt{x^2-1} \\
    y=\cfrac{1}{2+\cfrac{1}{2}}     \\
    y=\int \! (x^2-1) dx             \\
    y=\int (x^2-1) dx                \\
    y=\int_{a}^{b=10} (x^2-1) dx            \\
    y=\sum_{x=1}^ {100} (x^2-1)- 1          \\
    BER= erfc(\frac{Q}{\sqrt{2}})
    $$
    
    $$
    \fbox {this is a demo equation: }   \\
    BER= erfc(\frac{Q}{\sqrt{2}})
    $$

    ```
    $$
    y=\frac{1}{2} \times \sqrt{x^2-1} \\
    y=\cfrac{1}{2+\cfrac{1}{2}}     \\
    y=\int \! (x^2-1) dx             \\
    y=\int (x^2-1) dx                \\
    y=\int_{a}^{b=10} (x^2-1) dx            \\
    y=\sum_{x=1}^ {100} (x^2-1)- 1          \\
    BER= erfc(\frac{Q}{\sqrt{2}})
    $$
    
    $$
    \fbox {this is a demo equation: }   \\
    BER= erfc(\frac{Q}{\sqrt{2}})
    $$
    ```


