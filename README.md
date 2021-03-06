
### Online Preview Demo

First, take a look at the Online Demo:

1. A simplest Demo: [**http://www.ciaoshen.com/jekyll_bootstrap_shen_scroll/**](http://www.ciaoshen.com/jekyll_bootstrap_shen_scroll/)

![simpleDemo](/images/simpleDemo.png)

2. My personal web site: [**http://www.ciaoshen.com/thinkinginjava/**](http://www.ciaoshen.com/thinkinginjava/)

![mySite](/images/mySite.png)

### What is Jekyll Bootstrap Shen Scroll?

**Jekyll Bootstrap Shen Scroll** is a personal blog Template created for developers who want to
focus on the content instead of waste time on CSS stylesheet.


It merge both the **Jekyll** and **Bootstrap** to generate a static web site. Jekyll is a static blog scaffold, and Bootstrap randering the stylesheet for you.


Write your markdown articles, put them in a folder, and then generate your web site with one command line. And that's all!

### Jekyll

Jekyll is a blog scaffold that transform your plain text into static websites and blogs. For more useful detailed informations, please visit [**《Jekyll Online Document》**](https://jekyllrb.com/docs/home/).

And here are some interesting articles:
1. [<< a simple jekyll guide >>](http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html)
2. [<< jekyll structure >>](http://hustlei.tk/2014/08/jekyll-dir-and-config.html)
3. [<< the variables in jekyll >>](http://jekyllcn.com/docs/variables/)
4. [<< the collections in jekyll >>](http://jekyllcn.com/docs/collections/)

#### Jekyll Structure

This template use the simplest Jekyll structure as follow. But since Jekyll is highly scalable, you can expend any module whenever you want.

```bash
├── _config.yml
├── _layouts
|   ├── main.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-your-article-one.md
|   └── 2009-04-26-your-article-two.md
├── _site
├── assets
|   ├── css
|   └── fonts
|   └── js
├── .jekyll-metadata
└── index.html
```

An overview of what each of these does:

* **`_config.yml`**: This is the config file using YAML protocol. Most of the common arguments are included.
* **`_layouts`**: These are the templates that wrap posts. Layouts are chosen on a post-by-post basis in the YAML Front Matter. I initiate only two templates: one for main page, another for posts.
* **`_site`**: This is where the generated site will be placed (by default) once Jekyll is done transforming it. It’s probably a good idea to add this to your ".gitignore" file.
* **`assets`**: This is where I put the Bootstrap. You can see three folders: css,fonts and js.
* **`.jekyll-metadata`**: This is where the generated site will be placed (by default) once Jekyll is done transforming it. It’s probably a good idea to add this to your ".gitignore" file.
* **`index.html`**: The main access of your web site.


#### Liquid Template Language

Jekyll use the **Liquid Template Laguage** to process the markdown files in batches. Here is good online guide for Liquid: [**《Syntax of Liquid Template Language》**](https://github.com/shopify/liquid/wiki/liquid-for-designers)


To create some new Collections like `posts`, just add some add them into the `_config.yml` config file, and create a new directory `_your-new-collection` in the root of your project.

```bash
collections:
  posts:
    output:   true
  your-new-collection:
    output:   true
```

### Bootstrap
Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web. For more information please visit: http://getbootstrap.com/getting-started/

And here are some interesting articles:
1. [<< the subtle magic behind why the bootstrap 3 grid works >>](http://www.helloerik.com/the-subtle-magic-behind-why-the-bootstrap-3-grid-works)
2. [<< simplest sass guide >>](http://www.w3cplus.com/sassguide/)
3. [<< what is node.js >>](https://www.ibm.com/developerworks/cn/opensource/os-nodejs/)

#### Structure

The bootstrap library is  under the `assets` folder including three main directories: `css`, `fonts` and `js`.

```bash
assets
├── css
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   ├── rouge.css
│   ├── rouge_monokai.css
│   ├── rouge_monokai_original.css
│   └── scrolling-nav.css
├── fonts
│   ├── glyphicons-halflings-regular.eot
│   ├── glyphicons-halflings-regular.svg
│   ├── glyphicons-halflings-regular.ttf
│   ├── glyphicons-halflings-regular.woff
│   └── glyphicons-halflings-regular.woff2
└── js
    ├── bootstrap.js
    ├── bootstrap.min.js
    ├── imgResponsive.js
    ├── jquery.easing.min.js
    ├── jquery.js
    ├── mainDescriptionDiv.js
    ├── scrolling-nav.js
    ├── span.js
    └── spanPost.js
```

All the above files mixed three libraries together:
* original bootstrap library
* Scrolling Nav library
* my additionl library

##### Bootstrap original library

The following files are the original bootstrap library:

```bash
assets
├── css
│   ├── bootstrap.css
│   ├── bootstrap.min.css
├── fonts
│   ├── glyphicons-halflings-regular.eot
│   ├── glyphicons-halflings-regular.svg
│   ├── glyphicons-halflings-regular.ttf
│   ├── glyphicons-halflings-regular.woff
│   └── glyphicons-halflings-regular.woff2
└── js
    ├── bootstrap.js
    ├── bootstrap.min.js
```

##### Scrolling Nav library

A basic, unstyled Bootstrap page layout for creating smooth scrolling, one page websites. For more information, please visit:  https://startbootstrap.com/template-overviews/scrolling-nav/

**Usage Instructions** : Make sure to include the `scrolling-nav.js`, `jquery.easing.min.js`, and `scrolling-nav.css` files. To make a link smooth scroll to another section on the page, give the link the `.page-scroll` class and set the link target to a corresponding ID on the page.

The library structure is shown as follow. Note: Scrolling Nav cannot work without Bootstrap.

```bash
assets
├── css
│   └── scrolling-nav.css
└── js
    ├── bootstrap.js
    ├── bootstrap.min.js
    ├── jquery.easing.min.js
    ├── jquery.js
    ├── scrolling-nav.js
```

##### My Additional library

In the following files, `rouge.css`, `rouge_monokai.css`, `rouge_monokai_original.css` are the rouge code highlighter stylesheet. And I have made some changes in `scrolling-nav.css`.

```bash
assets
├── css
│   ├── rouge.css
│   ├── rouge_monokai.css
│   ├── rouge_monokai_original.css
│   └── scrolling-nav.css
└── js
    ├── imgResponsive.js
    ├── mainDescriptionDiv.js
    ├── span.js
    └── spanPost.js
```

`span.js` and `spanPost.js` is for adding some additional space between two `<h3>` and `<h4>` sections. `imgResponsive.js` makes the image size responsive to the different screen. `mainDescriptionDiv.js` adjusts the size of the description div.

### Usage

All stylesheets are already included in the template.

Use `h3` as the Level 1 title. `h4` as the sub title.

Give each Exercise page a following head:

```bash
layout: post
num: 1
title: Exercise 1
chapter: Chapter 11
description: >
  (2) Create a new class called Gerbil with an int gerbilNumber that’s initialized in the constructor. Give it a method called hop( ) that displays which gerbil number this is, and that it’s hopping. Create an ArrayList and add Gerbil objects to the List. Now use the get( ) method to move through the List and call hop( ) for each Gerbil.
```

Descriptions are recommended to be put in `<blockquote>` tag. If you want the descriptions section can scroll when they are too long, just give the div outside a class `description`, the javascript in template will do it for you.

#### Responsive grid

If you need a responsive column, defind the display rules using `col-xs-x`, `col-sm-x`, `col-md-x`, `col-lg-x` as follow.
```html
<div class="col-md-6 col-sm-6 col-xs-12 description">
```

The "Hamberger Button" is used to collapse the navigation bar.
```html
<button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-ex1-collapse">
    <span class="sr-only">Toggle navigation</span>
    <span class="icon-bar"></span>
    <span class="icon-bar"></span>
    <span class="icon-bar"></span>
</button>
```

### Contact Me

**Copyright**: MIT

**e-Mail**: symantec__@hotmail.com

**GitHub**: helloShen
