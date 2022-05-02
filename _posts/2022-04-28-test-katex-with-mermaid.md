---
layout: post
title: "test mathjax with mermaid"
categories: mermaid math
mermaid: forest
math: katex
author:
- jeffatoptics
---

katex equation and mermaid in `mermaid: forest` theme

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

<div class="mermaid"> 
graph TD; 
A-->B; A-->C; B-->D; C-->D; 
</div>  


<div class="mermaid">
graph LR;
  A-->B;
</div>



<div class="mermaid">
graph LR
A(This is A)----->|this is demo text|B[(this is database<br><br> demo)]
C((This is C))--this is demo text--->B
D{This is D}--this is demo text--->B

    subgraph box
        A---C----D
        subgraph newbox
        C
        D
        end
    end
    subgraph box2
    B
    end
style B fill:#bbf,stroke:#000,stroke-width:4px,color:#f00,stroke-dasharray: 10 2
linkStyle 0 stroke:#f00,stroke-width:4px
</div>


<div class="mermaid">
sequenceDiagram 
    participant Local
    participant Remote
    Local-xRemote: LOS is detected
    Note right of Remote: LOS will triger RFI
    Remote->>Local: RFI
    Local->>Remote: Idle 
    Note left of Local: RFI will stop transmission <br> and triggers idle
    
    Local-->>Remote: LOS clear
    Note right of Remote: idle is received <br> after LOS clear
    Remote->>Local: Data
    Local->>Remote: Data
</div>

## links

- [test katex](./2022-04-30-test-equation-katex.md)

- [mathjax test](2022-04-29-test-equation-mathjax.md)
