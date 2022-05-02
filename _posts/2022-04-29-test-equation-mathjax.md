---
layout: post
title: "test equation in mathjax"
categories: markdown
math: mathjax
author:
- jeffatoptics
---

test latex

$$
K(a,b) = \int \mathcal{D}x(t) \exp(2\pi i S[x]/\hbar)
$$

test latex


$ e = m c^2 $


inline: $f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$
inline: $$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$

display mode (centered):


$$ f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi $$


$$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$


$$
y=\frac{1}{2} \times \sqrt{x^2-1} \\
y=\cfrac{1}{2+\cfrac{1}{2}}     \\
y=\int \! (x^2-1) dx             \\
y=\int (x^2-1) dx                \\
y=\int_{a}^{b=10} (x^2-1) dx            \\
y=\sum_{x=1}^ {100} (x^2-1)- 1          \\
BER= erfc(\frac{Q}{\sqrt(2)})
$$
 
$$
\fbox {this is a demo equation: }    \\
BER= erfc(\frac{Q}{\sqrt(2)})
$$



```html
<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>
```