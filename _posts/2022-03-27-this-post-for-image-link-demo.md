---
layout: post
categories: work
title: demo a image as summary
---

![link demo]({{ site.baseurl }}{% link assets/images/dolphin.jpg %})

`{% raw %}![link demo]({{ site.baseurl }}{% link assets/images/dolphin.jpg %}){% endraw %}`

![](../assets/images/dolphin.jpg)

`![](../assets/images/dolphin.jpg)`

above is asset-folder reference with markdown syntax, it works.

**do not put the images and files in `_posts` folder. this do not works in github pages.**


![](../assets/images/dolphin.jpg){: width="250"}

`![](../assets/images/dolphin.jpg){: width="250"}`


<img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>
<img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>
<img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>
<img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>

`{% raw %}<img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=250/>{% endraw %}`
