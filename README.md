---
layout: page
permalink: readme.html
title: support math and mermaid diagram in jekyll/minima theme
---

Demo link: [https:// jeffatoptics.github.io/jeff-minima/](https://jeffatoptics.github.io/jeff-minima/)

## Purpose

Enhance [jekyll/minima](https://github.com/jekyll/minima) template with the support of **katex/mathjax** equation and **mermaid** diagram:

- enable **katex /mathjax** math support with `math: katex` or `math: mathjax` in page front matter.  disable with removing the above words.

- enable the **mermaid** support with `mermaid: default` `mermaid: dark` `mermaid: base` or `mermaid: neutral`  or nothing in page front matter.  disable with removing the above words. 

- make a [category page](./category.md) to auto display the notes by their category attributes

## Major changes from the [jekyll/minima](https://github.com/jekyll/minima)


1. add the codes in **[custom-head.html](_includes/custom-head.html)** to support katex/mathjax and mermaid in `_includes` folder

1. add a [category page](./category.md)

There are also minor changes of theme layout and color:

- set the minima content-width to 1000px: `$content-width` in [`./_sass/minima/initialize.scss`](./_sass/minima/initialize.scss). The default was 800px

- adjust the dark scheme font `$text-color` in [`./_sass/minima/initialize.scss`](./_sass/minima/initialize.scss) to lighter value as `eeeeee`. `$brand-color-light` lighter is adjusted from 5% to 35%


## Usage

1. copy all the files to the local folder.
1. customizing the `author name` `email` `description` `skin` in `_config.yml`. skin are typically `default` or `dark`.
1. customizing the `index.md`
1. delete the markdown template files in `_posts` folder, and input your own markdown with proper naming "yyyy-mm-dd-topic.md"
1. delete the images in `assets` folder, and put your own, and link them with `_post` markdown files
1. remove or customize the md files in root, i.e. [about.md](about.md) [header1.md](header1.md) [readme.md](readme.md) and [index_simple.md]

## Syntax

1. katex  is using `$ <latex> $` as inline equation, `$$ <latex> $$`  or 

```

$$
<latex>
$$

``` 

for math block. katex is quicker than mathjax. 

2. mathjax is using `$ <latex> $` and `$$ <latex> $$` for inline, and

```
$$
<latex>
$$
``` 

3. mermaid is using the following syntax with `<div>`.

```html
<div class="mermaid">
graph LR;
 A-->B;
</div>
```
> 📑 **link syntax recommendation**

jekyll liquid syntax always works, but I would recommend to use markdown relative syntax as much as possible. 
>- Examples:
>    - `[link to a file in post](./_posts/2022-04-26-this-post-demonstrates-post-content-styles.md)`
>    - `![link to a file in asset](../assets/images/dolphin.jpg)`
>    - `![](../assets/images/dolphin.jpg){: width="250"}`  
