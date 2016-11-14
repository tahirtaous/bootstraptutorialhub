---
layout: post
title: Getting Started With Bootstrap Tutorial for beginners
date: 2016-11-11 10:55:54 +0500
categories: bootstrap
image: /assets/images/getting-started-with-bootstrap.png
excerpt: In this Bootstrap tutorial, you will learn how to get started with Bootstrap framework.
---

<img src="{{site.baseurl}}/assets/images/getting-started-with-bootstrap.png" alt="Getting Started With Bootstrap Tutorial for beginners">

To use Bootstrap framework, basic understanding of HTML and CSS is necessary. But if you don't anything about HTML, CSS, you should learn basics of HTML and CSS.

There are many free ebooks available to learn HTML and CSS. Read this tutorials to find a list of [Free HTML and CSS Books](http://justlearnwp.com/free-web-design-books-pdf-download/).

## Download and Set up Bootstrap

One of the best way to learn and use bootstrap is, download Bootstrap framework and practice.

Visit [getbootstrap.com](http://getbootstrap.com/) and click on Download Bootstrap button to downlod all the code.

When toy will click on Download Bootstrap button, you will be redirected to *Getting Started* http://getbootstrap.com/getting-started/#download page.

You will see different download and install options.

- **Download Bootstrap** : Compiled and minified CSS, JavaScript, and fonts. No docs or original source files are included.
- Download Source
- Download Sass
- Bootstrap CDN
- Install with Bower
- Install with npm
- Install with Composer

if you are always connected to Internet, you can use Bootstrap CDN version, but I recommend Compiled and minified CSS, JavaScript, and fonts version.

> If you want to see all examples and documentation, click on DOWNLOAD SOURCE button. 

Use any program to extract all files from the zipped archive, you just downloaded. Name of extracted folder will be something like `bootstrap-3.3.7-dist`. Here 3.3.7 is the version number of Bootstrap.

Under primary folder, you can see three sub folders.

- css
- fonts
- js

Above folder contains all the Bootstrap CSS, JavaScript and Icon font files. In this folder create a new file and save it is `index.html`. This will be the main page of your site.

I use [SublimeText](https://www.sublimetext.com/) a very popular code editor to edit HTML, CSS and other files. Code Editors like sublime text offer syntax highlighting, error reporting, auto complete and other advance features.

Now open Index.html file and add following [basic](http://getbootstrap.com/getting-started/#template) page markup in this file.

{% highlight css %}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <title>Bootstrap 101 Template</title>

    <!-- Bootstrap -->
    <link href="css/bootstrap.min.css" rel="stylesheet">

    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
    <!-- Include all compiled plugins (below), or include individual files as needed -->
    <script src="js/bootstrap.min.js"></script>
  </body>
</html>
{% endhighlight %}

Open this file in your favorite browser. Chrome and Firefox are very popular browser.

Now lets create a very simple two-column website with primary navigation and a featured content area.

Replace `<h1>Hello, world!</h1>` with following markup.

{% highlight html %}
<div class="container">

nav here

feature area

Two column area

</div> <!-- end ##container -->
{% endhighlight %}

Bootstrap has a responsive grid system. With this grid system, you can create multi-column layouts quickly and easily.

In above example, first we have a div `<div class="container">` with class of container. This class creates a outer container for all site content.

### Main Navigation

First of all we are going to add primary navigation menu to our site. Replace **nav here** with the following markup.

{% highlight html %}
<ul class="nav nav-tabs">
  <li class="active"><a href="index.html">Home</a></li>
  <li><a href="about.html">about</a></li>
  <li><a href="contact.html">contact</a></li>
</ul>
{% endhighlight %}

#### Result

<ul class="nav nav-tabs">
  <li class="active"><a href="index.html">Home</a></li>
  <li><a href="about.html">about</a></li>
  <li><a href="contact.html">contact</a></li>
</ul>

save your changes and open your file in browser. You can see that HOME link is highlighted because we have used `class="active"` on th first link.

## Featured content area

Now lets add featured content area. Bootstrap has a `.jumbotron` class, which you can use to create a featured content area where, which you can use to showcase key content on your site.

Now replace `feature area` with the following markup.

**Code**

{% highlight html %}
<div class="jumbotron">
  <h1>My Awesome Product</h1>
  <p>...</p>
  <p><a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a></p>
</div>
{% endhighlight %}

**Result**
<div class="container">
    <div class="jumbotron">
  <h1>My Awesome Product</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt ea nihil, ipsa itaque obcaecati iure architecto sequi distinctio dicta.</p>
  <p><a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a></p>
</div>
</div>

## Two columns layout

To create multi-columns layout, you can use `col-md-*` class (md= medium grid). You can replace `*` with your desired number from 1-12, because bootstrap has 12 column grid system.

If you want two column layout, first wider column for primary content area and second small column for sidebar content, You need to use following markup.

{% highlight html %}
<div class="row">
    <div class="col-md-8">
      Wider column for primary content area
    </div>
    <div class="col-md-4">
      column for sidebar content area.
    </div>
</div> <!-- end ##row -->
{% endhighlight %}

Above code will generate two column layout for your responsive website. Here you can see the result.

<hr>
<div class="row">
    <div class="col-md-8">
    <h3>Primary Content</h3>
      Wider column for primary content area. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatum voluptates, molestiae temporibus esse laboriosam perferendis tempora eligendi culpa reiciendis quod, sit dolor!
    </div>
    <div class="col-md-4">
    <h3>Sidebar</h3>
      column for sidebar content area.
    </div>
</div> <!-- end ##row -->
<hr>

## That's all

You have created your first responsive website with Bootstrap framework. You can also download final code files of this tutorial.

<a href="{{site.baseurl}}/assets/files/getting-started-bootstrap-files.zip">Download Tutorial File</a>