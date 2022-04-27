---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
title: HOME
layout: home
list_title: my-daily-note
---

<p align=center>
<img height=200 style="float:none" src="./assets/images/dophin.jpg" /></p>

[View Github repository](https://github.com/jeffatoptics/jeff-minima)

[link to a file in post](./_posts/2022-04-26-this-post-demonstrates-post-content-styles.md)

{% post_url 2022-04-26-this-post-demonstrates-post-content-styles %}
{{ site.baseurl }}{% post_url 2022-04-26-this-post-demonstrates-post-content-styles %}
[link demo]({% post_url 2022-04-26-this-post-demonstrates-post-content-styles %})