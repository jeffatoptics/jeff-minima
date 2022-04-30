---
layout: post
title: "test mermad"
categories: markdown
math: 
author:
- jeffatoptics
---

this is to test mermaid:

<script src="/assets/js/mermaid.min.js"></script>
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
<div class="mermaid"> graph TD; A-->B; A-->C; B-->D; C-->D; </div>

<script>
mermaid.init({noteMargin: 10}, ".language-mermaid");
</script>