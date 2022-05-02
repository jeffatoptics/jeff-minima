---
layout: post
title: "demonstrate links to markdown file in post folder"
categories: link syntax
author:
- jeffatoptics
---

>📝 Recommend to use the relative link markdown syntax

## Relative link markdown syntax  

- link to the file in root: [home](../index.md)

    ```
    [home](../index.md) 
    ```
    
- link to the file in _poster: [next](2022-03-27-image-link.md)

    ```
    [next](2002-04-21-test-date.md)
    ```



## jekyll link syntax

refer to [jekyllrb doc](https://jekyllrb.com/docs/liquid/tags/)

- [home url]({{ site.url }})
    ```
        {% raw %}
        [home url]({{ site.url }})
        {% endraw %}
    ```


- [home base url]({{ site.baseurl }})
    ```
    {% raw %}
    [home base url]({{ site.baseurl }})
    {% endraw %}
    ```


- [post link demo]({{ site.baseurl }}{% post_url 2022-03-26-markdown-content-styles %}): link to file in _posts
    ```
    {% raw %}
    [post link demo]({{ site.baseurl }}{% post_url 2022-03-26-markdown-content-styles %})
    {% endraw %}
    ```
- [link to root file ]({{ site.baseurl }}{% link header1.md %}): link to file in root
    ```
    {% raw %}
    [link to root file ]({{ site.baseurl }}{% link header1.md %})
    {% endraw %}
    ```

## jekyll variable values

- baseurl value: {{ site.baseurl }}

    ```
    {% raw %}
    baseurl value: {{ site.baseurl }}
    {% endraw %}
    ```
- url value: {{ site.url }}
    ```
    {% raw %}
    url value: {{ site.url }}
    {% endraw %}
    ```

[image link demo](2022-03-27-image-link.md)

