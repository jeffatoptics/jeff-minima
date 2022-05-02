---
layout: post
title: "link demo in post folder"
categories: link syntax
author:
- jeffatoptics
---

Recommend to use the relative link markdown syntax 

## Relative link markdown syntax  

- [home](../index.md) 
- [next](2022-03-27-image-link-demo.md)

```
- [home](../index_image.md) 
- [next](2002-04-21-test-date.md)
```



## jeklly link also works 


- [home url]({{ site.url }})

- [home base url]({{ site.baseurl }})

- [post link demo]({{ site.baseurl }}{% post_url 2022-04-26-this-post-demonstrates-post-content-styles %})

- baseurl value:{{ site.baseurl }}

- url value: {{ site.url }}

- [back](2022-03-26-markdown-content-styles.md) 
- [next](./2022-04-27-example2%20.md)