---
layout: post
title: Jekyll with github pages
lang: en
lang-ref: jekyll-github-pages
tags:  [jekyll, github pages]
---

[GitHub pages](https://pages.github.com/) is a fast, confortable and powerful
solution if you need a simple homepage. In addition to that it's fully integrated
with github environment.

In the beginning you should create a simple repository with this naming convention: *$username.github.io* 
Although this works out of box, you can have more! [jekyll](https://jekyllrb.com/) 
site generator can support more dynamic solutions.

This blog is based on that.

<!-- more -->
[This page on github](https://github.com/lsmhun/lsmhun.github.io)

This blog template is based on [István Viczián](www.jtechlog.hu) example. I wanted to write 
blog posts in English and Hungarian, so I had to change some points.

Jekyll has a lot of modules, but Github Pages supports just few of them: 
[supported versions](https://pages.github.com/versions/). Of course
[Multi languages plugin](https://github.com/kurtsson/jekyll-multiple-languages-plugin) is not on the list. 
Sad face included...

There are some good articles about multi language support with Jekyll:
- [KlaasNotFound](https://www.klaasnotfound.com/2017/02/16/proper-multilingual-site-with-github-pages-and-jekyll/)
- [brendamour](https://brendamour.net/2014/08/03/multilingual-jekyll-how-to-post-in-more-than-one-language/)

Imho documentation belongs to the code base, and it should be as close as possible to the real
working system, plus it should be generated if possible. As a result I wrote my short 
dev notes in *docs* directory in my example projects. I hoped that there is a solution for that.
Actually there is a [remote include plugin](https://github.com/netrics/jekyll-remote-include), but 
it's not on the supported list neither. So I stayed with copy-paste... Shame! Shame!

There could be a third, more professional solution: you can build your own CI pipeline for the page. 
I found a good [blog post](https://github.blog/2022-02-02-build-ci-cd-pipeline-github-actions-four-steps/),
but I didn't implement it. Last option could be the poor man's CI, when you build and run your 
page locally with all of the plugins and publish just the result *_site* directory. It's the worst and
ugliest option, so I drop the idea. 

Language selection could be cleaner, not just a link to english/hungarian main page. In meta data I added
*lang-ref* and it could link directly between translations (this is supported by the multilang plugin).
Nevertheless I doubt that anyone will read the same thing in two languages. I added just a simple
browser lang based forwarder script. SEO experts will cry in the corner, because search robots will
punish it in scores. 

If I would register a domain then it's easy to activate it with a *CNAME* file in root directory. Domain(s)
can be written there and after that {{ BASE_PATH }} template variables will use this. 
Out of box supported, simple and elegant.

