---
layout: page
permalink: readme.html
title: A simplified minima template
---

## purpose

- simplify the [jekyll/minima](https://github.com/jekyll/minima), and use these files as template

- auto display the posts (dailynote) per date-time, and a category page summrizing the posts (dailynote) by category

- write markdown file locally, and push to github

<img src="https://pic4.zhimg.com/80/v2-bb3a7c4188c8ccc6b1fdcf356c823f24.gif" alt="jeff-minima" width=800>

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
1. customizing the `author name` `email` `description` in `_config.yml`
1. customizing the `index.md`
1. move/delete the templated files from `_posts` folder after you read the link syntax
1. input the markdown files to `_posts`  folder

## link syntax recommendation

- use markdown syntax rather than jekyll.

    - `[link to a file in post](./_posts/2022-04-26-this-post-demonstrates-post-content-styles.md)`

    - `![](../assets/images/dophin.jpg)`

    - `![](../assets/images/dophin.jpg){: width="250"}`