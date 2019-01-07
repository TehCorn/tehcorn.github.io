---
layout: post
title:  "My First Jekyll Post"
date:   2019-01-07 17:44:50 -0500
categories: jekyll update install post
---

[GitHub Pages](https://pages.github.com/) is a way to host static HTTP sites through a GitHub repository. Here's a quick run-down of how to get shit up and running in Jekyll.

## Ubuntu Installation
(Alternatively, just visit the [Jekyll Docs](https://jekyllrb.com/docs/installation/ubuntu/))

Jekyll runs in Ruby, so you will need to make sure you have a full Ruby development environment set up. For Ubuntu, this means:

```
sudo apt-get install ruby-full build-essential zlib1g-dev
```

With those packages, you can use `rubygems` to install `jekyll` and `bundler`, as follows:

```
sudo gem install jekyll bundler
```

Then just run `jekyll new pathname` to create a directory for the Jekyll site.


## Config and Themes

GitHub Pages supports a [limited number of Themes](https://pages.github.com/themes/) but you can also [Add your own themes](https://help.github.com/articles/adding-a-jekyll-theme-to-your-github-pages-site/) following the directions linked.

This blog initially was created with the [Midnight Theme](https://github.com/pages-themes/midnight) by adding to the `_config.yml` file:

```
theme: jekyll-theme-midnight
```

**Important** you must also add the correct rubygem in your `Gemfile` and then run `bundle` to see the CSS.


## Markdown

All Jekyll Markdown files will contain a YAML text block at the top of the file known as [Front Matter](https://jekyllrb.com/docs/front-matter/) that is set apart from the rest of the file by two triple-dashed lines.

For more info on Jekyll project directory structure check [here](https://jekyllrb.com/docs/structure/). In short, all non-special files/directories (and non-markdown) will be copied verbatim to the generated site, so be aware of what you stick in your Jekyll project directory.


## Assets Demo

Demo for displaying assets. See image below:

![DAZ](/assets/images/testdaz.png)
