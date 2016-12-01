---
layout: post
title: A brief introduction to bootstrap 3 framework features
date: 2016-11-11 10:55:54 +0500
categories: bootstrap
image: /assets/images/bootstrap3-features.png
excerpt: In this Bootstrap tutorial, you will learn how to get started with Bootstrap framework.
---

<img src="{{site.baseurl}}/assets/images/bootstrap3-features.png" alt="Getting Started With Bootstrap 3 Features">

**Requirements**: Bootstrap Version: 3.3.7

[Bootstrap][1] is a front end development framework to create beautiful, fully responsive websites. It was created by Mark Otto and Jacob Thornton, who were designer and developer at [Twitter.com][2].

initially Bootstrap was called twitter Blueprint, when it was first created in 2010. In August, 2011 Bootstrap was released as an open-sourced framework.

In version 2, bootstrap team added responsive functionality to the entire framework as an optional style-sheet. Version 3 of bootstrap was a major release, complete library was rewritten to make Bootstrap fully responsive by default.

Front-end refers to the client side of website, that's the part of a website a visitor sees in the browser. A front-end development framework is a bunch of code that is written for you already, that you can use to build great websites quickly and easily without learning a lot of code.

Twitter Bootstrap has a [comprehensive documentation to get started][3] in English. Community members have translated Bootstrap's documentation into Chinese, Spanish and Russian languages. None are officially supported by Twitter Bootstrap and may not always be up to date.

*   [Bootstrap 中文文档 (Chinese)][4]
*   [Bootstrap по-русски (Russian)][5]
*   [Bootstrap en Español (Spanish)][6]

## Why You should use Twitter Bootstrap ?

You will be able to create beautiful and fully responsive website quickly and easily without learning a lot of coding, best practices and CSS3 media Queries from scratch. Media Queries used to make your static websites responsive.

You can learn Bootstrap in a few days but it will take months or years to be an expert in HTML, CSS, Responsive design and JavaScript. Writing code is not difficult but writing bug free, semantic code with industry's best practices that will work on different platforms is a really difficult.

## Twitter Bootstrap Features

### CSS Styles

Twitter Bootstrap is mobile first, it means your websites will be fully responsive on desktop, tablets and smart phones. You can make images responsive by adding `.img-responsive` class in bootstrap 3. For improved cross-browser rendering, Bootstrap uses [Normalize.css][7], a project by [Nicolas Gallagher][8] and [Jonathan Neal][9].

### Responsive Grid System Twitter Bootstrap

Twitter Bootstrap has a 12 column responsive, mobile first grid system, which uses predefined classes like `.container` to create a primary wrapper for your web page, `.row .col-xs-4, .col-md-1, col-md-4` and others to create grid layouts quickly and easily.

You can use `.col-xs-*` to target small screen devices such as mobile phones, `.col-md-*` will target medium devices like tablets, desktop and `.col-lg-*` will target large screens. ** * ** will be replaced with your desired number for grid layout.

For example you can create 2 column layout easily with `.col-md-8` for main area and `.col-md-4` class for sidebar.

Twitter Bootstrap Classes are available for Mobile, tablets and desktops. With Twitter Bootstrap's these classes you can easily create multi column layouts.

Advance users can use LESS mixins to create more semantic layouts. For example to create a 2 column layout you can use following code.

{% highlight HTML %}
    <div class="container">
    
        <main class="row">
    
            <article class="col-md-8">
               primary content
            </article> <!--end .col-md-8-->
    
            <aside class="col-md-4">
                sidebar content
            </aside><!--end .col-md-4-->
    
        </main> <!--end .row-->
    
    </div> <!--end .container-->
{% endhighlight %}

### Typography in Twitter Bootstrap

Bootstrap offers many classes to style heading, text, paragraphs etc. Alignment classes `.text-left, .text-center, .text-right` allows you to easily realign text s with available text alignment classes.

Emphasis classes `.text-muted, text-primary, .text-success` and other classes will color your text. styling for lists, block quotes, code is also available.

### Tables styling in Twitter Bootstrap

Creating and styling tables are very easy with bootstrap, you can apply `.table-striped, .table-bordered, .table-hover, .table-condensed` to apply styling to whole table or use contextual classes `.active .success .warning` and `.danger` to color table rows or individual cells.

### Making Tables Responsive

Creating responsive tables is simple by wrapping any `.table` in `.table-responsive` to make them scroll horizontally up to small devices (under 768px).

### Forms in Twitter Bootstrap

Creating different type of form with bootstrap is also simple and easy. Since version 3 of Twitter Bootstrap inputs, selects, and textareas are 100% wide by default in Bootstrap framework.

You can use predefined grid classes to align labels and groups of form controls in a horizontal layout. Form states will allow you to provide feedback to users.

### Buttons and images

Creating beautiful buttons are easy just apply available classes to change the size, color or state. There are many classes available to style buttons, such as .btn-primary will make your button blue, .btn-success will add green background and btn.danger will add red background to your button.

Even `.btn-lg`, `.btn-sm`, `.btn-xs` and `.btn-block` are available to make buttons large, small, extra small and block.

Bootstrap offers `.img-rounded`, `.img-circle` and `.img-thumbnail` to style images. These classes will make your images square, round and add border to your images.

Image replacement is simple just apply `.text-hide` class to replace an element's text content with a background image for example for site logo.

### Faster mobile-friendly development with Responsive utilities

One of the cool feature of bootstrap was the ability to mark the content so that it only appears in certain devices. That remains in the new version but class names has been changed in version 3.

Bootstrap 3 offers 8 different classes to show or hide content from screen. For example if you apply `.visible-xs` to an element, it will only be visible on extra small devices Phones (<768px) and hidden on tablets and desktops.

print classes are also available for toggling content for print. You can use `.visible-print` to show and `.hidden-print` class to hide content while printing. Components

## Pre built Components

Pre built components are one of the most cool feature of Bootstrap. Many components are available to make your work flow faster, which includes drop downs, button groups, navigation menus, breadcrumbs, pagination, labels, thumbnails, alerts and many others.

Lets have a look at some of them in details.

### Glyphicons

Since version 3 bootstrap included 200 glyphs in font format. It is a welcome change because they can be resized and will display perfectly even if the resolution of the screen increases.

It also gives you the ability to color icons, before version 3 of twitter bootstrap you can only use white or black version of icons.

### Dropdown and Navigation Menus

Bootstrap uses drop-down JavaScript plug-in for drop down items. Drop down can be used with buttons and nav menus. There are many nav menus available in Bootstrap that can be styled differently with `.nav-pills`, `.nav-tabs`, `.nav-stacked`. and `.nav-justified`. You can use `.nav-justified` make tabs or pills equal widths of their parent at screens wider than 768px .

### Jumbotron and Thumbnails

Jumbotron is a big area usually spanning the width of web page. Jumbotron is great to draw user attention. It is main component for calling extra attention and to show featured content or information.

Thumbnail component can be used to easily display grids of images, videos, text, and more. Create products pages or use to show any related information. It is possible to add heading, paragraphs and buttons into thumbnails.

### List groups

List groups component lets you create mobile like lists with a lot of different options. You can create an unordered list with a class of `.list-group` and list-items with `.list-group-item` class. You can easily add badges to list items or make them click able links by making them into anchor tag..

### JavaScript and JQuery plugins

Bootstrap uses a number of JQuery based plug ins, JQuery is one of the most popular JavaScrit framework. These plugins includes Modals , Dropdowns, ScrollSpy, Tab, Tooltip, Popover, Carousel and many others. Carousal is one of the most popular feature of bootstrap. It can be used to create slide show of featured products or images.

### Twitter Bootstrap and Browser Support

Bootstrap will work best in the latest desktop and mobile browsers, older browsers might display differently styled, though fully functional, renderings of certain components. Twitter Bootstrap supports the latest version of [Chrome][10], [Safari][11], [Firefox][12], [Internet Explorer][13] and [Opera][14] browser.

According to official bootstrap documentation

> Unofficially, Bootstrap should look and behave well enough in Chromium and Chrome for Linux, Firefox for Linux, and Internet Explorer 7, though they are not officially supported.

### Internet Explorer 8 and 9

Internet Explorer 8 and 9 are also supported, however, some CSS3 properties and HTML5 elements are not fully supported in Internet Explorer 8 and 9 . Internet Explorer 8 does not support border-radius, box-shadow, transform, transition and placeholder.

Internet Explorer 8 requires the use of Respond.js to enable media query support. Respond.js is a fast & lightweight polyfill for min/max-width CSS3 Media Queries (for IE 6-8, and more).

## Download Twitter Bootstrap

### Download Pre Compiled Version

Bootstrap offers a lot of features. You can download pre compiled version at <http://getbootstrap.com/getting-started/>, which includes 3 folder CSS, Fonts and JS with minified and non minified files.

### Download Twitter Bootstrap with source code

You can download Source code directly from [github][15] with LESS, JavaScript source and example files. You can visit <http://getbootstrap.com/getting-started/> to download compiled and minified version, Less and Saas support is also available and you can download your desired version of Bootstrap as well.

[Visit github page][15]

[Visit getting started page][3]

### Customize and download

Evert project has different requirements, Not all components are required in every project, you can choose what you need, for example if you want to use Grid system only, you can visit Bootstrap's customize page and select components and features you want..

Visit [Twitter Bootstrap's customize page][16] select features you want and click Compile and download.

That's all. Twitter Bootstrap is very powerful framework, which makes your workflow much faster and easier. I use this framework to create responsive WordPress themes quickly, have you used this awesome framework, how do you use it, share your views in comments.

 [1]: http://getbootstrap.com/
 [2]: http://Twitter.com/TahirTaous
 [3]: http://getbootstrap.com/getting-started/
 [4]: http://v3.bootcss.com/
 [5]: http://www.oneskyapp.com/ru/docs/bootstrap
 [6]: http://www.oneskyapp.com/docs/bootstrap/es
 [7]: http://necolas.github.io/normalize.css/
 [8]: http://nicolasgallagher.com/
 [9]: http://www.jonathantneal.com/
 [10]: https://www.google.com/intl/en/chrome/browser/
 [11]: https://www.apple.com/safari/
 [12]: http://www.mozilla.org/en-US/firefox/new/
 [13]: http://windows.microsoft.com/en-us/internet-explorer/download-ie
 [14]: http://www.opera.com/
 [15]: https://github.com/twbs/bootstrap
 [16]: http://getbootstrap.com/customize/