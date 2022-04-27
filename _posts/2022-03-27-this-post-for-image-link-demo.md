---
layout: post
categories: note2
title: demo a image as summary
---

![](../assets/images/dophin.jpg)

`![](../assets/images/dophin.jpg)`

above is asset-folder reference with markdown syntax, it works.

**do not put the images and files in `_posts` folder. this do not works in github pages.**

![link demo]({{ site.baseurl }}{% link assets/images/dophin.jpg %})

`![link demo]({{ site.baseurl }}{% link assets/images/dophin.jpg %})`

![](../assets/images/dophin.jpg){: width="250"}

`![](../assets/images/dophin.jpg){: width="250"}`


<img src="{{ site.baseurl }}{% link assets/images/dophin.jpg %}" width=250/>

`<img src="{{ site.baseurl }}{% link assets/images/dophin.jpg %}" width=250/>`
