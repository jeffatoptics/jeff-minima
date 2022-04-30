---
layout: post
title: "test mermad"
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
graph LR;
  A-->B;
</div>

<!-- <script async src="https://unpkg.com/mermaid@8.2.3/dist/mermaid.min.js"></script> -->

<script async type="text/javascript"
  src="https://unpkg.com/mermaid@9.0.1/dist/mermaid.min.js">
</script>
<script>
$(document).ready(function() {
    mermaid.initialize({
        theme: 'forest'
    });
});
</script>
