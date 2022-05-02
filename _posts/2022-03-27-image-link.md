---
layout: post
categories: link syntax
title: demonstrate links to image file
---

1. `{% raw %}![link demo]({{ site.baseurl }}{% link assets/images/dolphin.jpg %}){% endraw %}`

    mixed with jekyll liquid syntax. 

    ![link demo]({{ site.baseurl }}{% link assets/images/dolphin.jpg %})

1. `![](../assets/images/dolphin.jpg)`

    markdown syntax. relative reference
    ![](../assets/images/dolphin.jpg)

1. `![](../assets/images/dolphin.jpg){: width="250"}`

    markdown relative link syntax with jekyll liquid for size definition. 
    ![](../assets/images/dolphin.jpg){: width="250"}

1. {% raw %} <img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>{% endraw %}

    html image syntax with jekyll liquid variables.
    absolute link reference
    <img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>
    <img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>
    <img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>
    <img src="{{ site.baseurl }}{% link assets/images/dolphin.jpg %}" width=225/>

[another demo in root folder](../demonstrate-links-in-root-folder.md.md)


> ⚠️ **Do not put the images and files in `_posts` folder.**
> **The relative links to static files (other than markdown file) do not works in github pages!**