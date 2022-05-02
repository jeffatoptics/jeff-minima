---
layout: post
title: "test equation in mathjax"
categories: math
math: mathjax
author:
- jeffatoptics
---

Test mathjax equation display as below:

$$
f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi
$$

> 📝 enable katex with front matter in current page:
> ```
> ---
> math: mathjax
> ---
> ```

1. math block:

    $$
    K(a,b) = \int \mathcal{D}x(t) \exp(2\pi i S[x]/\hbar)
    $$

    ```
    $$
    K(a,b) = \int \mathcal{D}x(t) \exp(2\pi i S[x]/\hbar)
    $$
    ```
1. math inline:

    this is inline function $f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$ and another inline function $ e = m c^2 $

    ```
    this is inline function $f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$ and another inline function $ e = m c^2 $
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

## links
- [test katex](./2022-04-30-test-equation-katex.md)
- [display mermaid and katex together](./2022-04-28-test-katex-with-mermaid.md)
