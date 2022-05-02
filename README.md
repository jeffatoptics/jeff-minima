---
layout: page
permalink: readme.html
title: Support math and mermaid in jekyll/minima theme
---

Demo link: [https://jeffatoptics.github.io/jeff-minima/](https://jeffatoptics.github.io/jeff-minima/)

## Purpose

Enhance [jekyll/minima](https://github.com/jekyll/minima) template with the support of **katex/mathjax** equation and **mermaid** diagram:

- Enable **katex /mathjax** math support with `math: katex` or `math: mathjax` in page front matter. Disable it by removing the above words.

- Enable the **mermaid** support with `mermaid: default` `mermaid: dark` `mermaid: base` or `mermaid: neutral` theme in page front matter.  Disable it by removing the above words. 

- make a [category page](./category.md) to auto display the notes by their category attributes

## Major changes from the [jekyll/minima](https://github.com/jekyll/minima)


1. Add the codes in **[custom-head.html](_includes/custom-head.html)** to support katex/mathjax and mermaid in `_includes` folder

1. Add a [category page](./category.md)



## Minor changes

They are related to the theme layout and color:

1. set the minima content-width to 1000px: `$content-width` in [`./_sass/minima/initialize.scss`](./_sass/minima/initialize.scss). The default was 800px

1. adjust the dark scheme font `$text-color` in [`./_sass/minima/initialize.scss`](./_sass/minima/initialize.scss) to a lighter value as `eeeeee`. it was `bbbbbb` `$brand-color-light` is adjusted from 5% to 35%

1. add an emoji favicon 🐬 in customer-head.html. you can change it to any emoji or remove the line `<link rel="icon"..`

1. copy the [sandervoerman/minima](https://github.com/sandervoerman/minima/blob/prefers-color-scheme/_sass/minima/skins/auto.scss) for auto theme support

## Usage

1. copy all the files to the local folder.
1. customizing the `author name` `email` `description` `skin` in `_config.yml`. skin are typically `classic`,`dark`,`solarized-dark` and `solarized`
1. customizing the `index.md`
1. delete the markdown template files in `_posts` folder, and input your own markdown with name "yyyy-mm-dd-topic.md"
1. delete the images in `assets` folder, and put your own, and link them with `_post` markdown files
1. remove or customize the md files in root, i.e. [about.md](about.md) [header1.md](header1.md) [readme.md](readme.md) and [index_simple.md]

## Syntax in your notes

1. katex  is using `$ <latex> $` as inline equation, `$$ <latex> $$`  and 

    ```
    $$
    <latex>
    $$
    ``` 
    for math block. 

1. mathjax is using `$ <latex> $` and `$$ <latex> $$` for inline, and

    ```
    $$
    <latex>
    $$
    ``` 
1. mermaid is using the syntax with `<div>`.

    ```html
    <div class="mermaid">
    graph LR;
    A-->B;
    </div>
    ```
1. link syntax recommendation
    jekyll liquid syntax always works, but I would recommend to use **markdown relative syntax** as much as possible to align to local markdown editor. Examples:
    - `[link to a file in post](./_posts/2022-03-26-markdown-content-styles.md)`
    - `![link to a file in asset](../assets/images/dolphin.jpg)`
    - `![](../assets/images/dolphin.jpg){: width="250"}`  
