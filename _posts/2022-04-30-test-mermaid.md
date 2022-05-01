---
layout: post
title: "test mermaid"
categories: markdown
mermaid: true 
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
%%{init: {'theme':'default', 'themeVariables': { 'lineColor': 'green' }}}%%
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
flowchart LR
A<==>B<-..->C
A[this is a text]
B[this is demo]
style B fill:#bbf

</div>

<div class="mermaid">
%%{init: {'theme':'dark', 'themeVariables': { 'lineColor': 'green', 'textColor': 'yellow' }}}%%
pie
    title Bugs in Software
    "transmission" : 15.00
    "alarm" : 25
    "management" : 66
    "performance" : 5
</div>

<div class="mermaid">
%%{init: {'theme':'dark'}}%%

gantt
    title A Gantt Diagram
    dateFormat  YY-MM-DD
    axisFormat   %y-%m-%d
    section Section 1
    A task           :done, a1, 21-12-01, 20d
    Another task     :active, after a1, 60d
    section Section 2
    B      :crit,22-02-12, 20d
    milestone: milestone,20d
</div>


<div class="mermaid">
%%{init: {'theme':'dark'}}%%

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
