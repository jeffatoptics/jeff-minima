---
layout: page
permalink: readme.html
title: A simplified minima template
---

## purpose

- simplify the [jekyll/minima](https://github.com/jekyll/minima), and use these files as template

- auto display the posts (dailynote) per date-time, and a category page summrizing the posts (dailynote) by category

- write markdown file locally, and push to github

<img src="https://pic4.zhimg.com/80/v2-b07de587e42e790c762525049052f332.gif" alt="jeff-minima" width=600>

## major changes from minima

1. remove all the unnecessary files

1. set content width  to 1280 px 
    ```
    $content-width:    1280px !default;
    $on-palm:          600px !default;
    $on-laptop:        1280px !default;
    ```
1. set the font text color to `"#dddddd"` in `dark.scss` , which is brighter than the default value `"#bbbbbb"`， also make `$brand-color-light` to lighter 15% from default 5%

1. add the [category.md](category.md) to show the posts in categories

1. set the skin to dark, `show_excerpts` to true

## usage

1. copy all the files to the local folder.
1. customizing the `author name` `email` `description` in `_config.yml`
1. customizing the `index.md`
1. move/delete the templated files from `_posts` folder after you notice the link syntax
1. input your markdown notes to `_posts`  folder with proper naming "yyyy-mm-dd-topic.md"

> 📑 **link syntax recommendation**
>- use markdown syntax rather than jekyll, which is easy for local mardown editor preview.
>-  `<img>` html syntax is not working in jekyll `_posts` folder. 
>- Examples:
>    - `[link to a file in post](./_posts/2022-04-26-this-post-demonstrates-post-content-styles.md)`
>    - `![](../assets/images/dophin.jpg)`
>    - `![](../assets/images/dophin.jpg){: width="250"}`  #comment `{width}` is not markdown syntax,but we have to use there to control the width