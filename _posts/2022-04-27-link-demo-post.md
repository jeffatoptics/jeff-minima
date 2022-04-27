---
layout: post
title: "link demo"
categories: note3
author:
- jeffatoptics
---

link demo with markdown syntax and jekyll syntax

## markdown link works 

- [home](../index.md) 
- [next](2002-04-21-test-date.md)


## jeklly link also works 


- [home url]({{ site.url }})

- [home base url]({{ site.baseurl }})

- [post link demo]({{ site.baseurl }}{% post_url 2022-04-26-this-post-demonstrates-post-content-styles %})

- baseurl value:{{ site.baseurl }}

- url value: {{ site.url }}