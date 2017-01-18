---
layout: empty
title: bootstrap
---

### Bootstrap
Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web. For more information please visit: http://getbootstrap.com/getting-started/

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

#### Bootstrap original library

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

#### Scrolling Nav library

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

#### My Additional library

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
