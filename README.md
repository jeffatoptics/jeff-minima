---
layout: page
permalink: readme.html
title: A simplified minima template
---

## purpose

simplify the [jekyll/minima](https://github.com/jekyll/minima), and use these files as template

   
## major changes from minima

1. remove all the unnecessary files

1. set content width  to 1280 px 
    ```
    $content-width:    1280px !default;
    $on-palm:          600px !default;
    $on-laptop:        1280px !default;
    ```
2. add the [category.md](category.md) to show the posts in categories

3. set the skin to dark, `show_excerpts` to true

## usage

1. copy all the files to the local folder.
1. customizing the `author name` `email` `description` in [_config.yml](_config.yml)
1. customizing the ``
1. move/delete the templated files from `_posts` folder after you read the link syntax
1. input the markdown files to `_posts`  folder
