---
layout: post
title: "test mermaid"
categories: markdown
math: 
author:
- jeffatoptics
---

this is to test mermaid:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

<div class="mermaid"> 
graph TD; 
A-->B; A-->C; B-->D; C-->D; 
</div>  


<div class="mermaid">
%%{init: {'theme':'forest', 'themeVariables': { 'lineColor': 'green'}}}%%
graph LR;
  A-->B;
</div>


<div class="mermaid">
%%{init: {'theme':'forest'}}%%
graph LR;
  A-->B;
</div>


<div class="mermaid">
%%{init: {'theme':'dark'}}%%
graph LR;
  A-->B;
</div>

<!-- <script async src="https://unpkg.com/mermaid@8.2.3/dist/mermaid.min.js"></script> -->

<script type="text/javascript"
  src="https://unpkg.com/mermaid@9.0.1/dist/mermaid.min.js">
</script>

<script>
mermaid.initialize({'theme': 'forest', 'themeVariables': {'lineColor': 'green'}});
</script>
