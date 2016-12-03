---
layout: post
title: How To Add Bootstrap Styling to MailChimp Sign up Forms?
date: 2016-11-13 10:49:54 +0500
categories: bootstrap 3
image: /assets/images/mailchimp-bootstrap-forms.png
excerpt: Learn how to create a naked MailChimp form (without styles) and style it with Bootstrap forms classes.
---

<img src="{{site.baseurl}}/assets/images/mailchimp-bootstrap-forms.png" alt="what is bootstrap framework">

<a title="Create a free mailchimp.com account" href="http://eepurl.com/bc2eND">MailChimp</a> is one of the most popular and widely used service for email marketing.

Creating email sign up forms, lists, managing your email subscribers and automating your email campaigns is very simple and easy with MailChimp.

<a href="{{site.baseurl}}/what-is-bootstrap">Bootstrap</a>
is most popular CSS framework to create fully responsive and mobile friendly websites.

Basic knowledge of HTML and CSS is required to use this awesome framework. You can <a href="{{site.baseurl}}/getting-started">build mobile friendly websites</a> very easily with Bootstrap framework.

But to be honest as a beginner it can be difficult to understand how to use so many awesome <a href="{{site.baseurl}}/bootstrap3-features">features Bootstrap provides</a> and services offered by MailChimp.

Mailchimp offers an easy to use sign up form builder, you can create customized email sign up forms.

In this article, I am going to show you how you can create a naked mailchimp signup form and add Bootstrap styling.

It is very simple and easy to add bootstrap form styling to mailchimp sign up forms.

## Create a Free MailChimp account

To get started with this tutorial you need a mailchimp account, if you don't have an account go and create a free <a title="Create a free mailchimp.com account" href="http://eepurl.com/bc2eND">MailChimp</a> account.

## Create a MailChimp List

After creating your free mailchimp account log in to your account. Click on lists and create a new list for your campaign or just type `https://us8.admin.mailchimp.com/lists/new-list/` in browser address bar to create a new list. Fill out all necessary details and save your list.

Now click on your List name and go to <strong>Sign up Forms</strong> to create a new sign up form for your mailing list. You will see following four options to create a form.

- General Forms
- Embedded Forms
- Subscriber popup
- Form Integration

We are going to create an embedded form, so click on Embedded form, you will see following options for forms.

- Classic Super
- Slim
- Naked
- Advanced

Select Naked. By default there are 3 fields for your sign up forms.

First name, Last Name and email. email field is required and other fields are not necessary. If you want a super simple and minimal form then check on <strong>Show only required fields</strong> radio button.

If you want all 3 fields than copy all the necessary mark up for your sign up form <strong>Copy/paste onto your site</strong> area. If you want to remove any field such as Last Name then click on the form builder link below Show only Required fields section.

### How to delete First or Last Name from MailChimp sign up form

I wanted to use First Name and email fields for my sign up form so i deleted Last Name field from my sign up form. To delete Last Name or any other field select that input field with mouse. You will see + and - symbols below selected input field.

To delete field click on - symbol and type DELETE in capital letters. It is must otherwise you can not delete any field from your sign up form.

When you will select any input field such as first name, last name or email field, on the right hand side you can see all field settings. For example if you will select First Name field, you can edit Field label and  field tag.

Default Field label for First Name is First Name, you can change this to Your Name or something you want. Field tag is used for Name tag in input form field, but leave this field as it is.

You can also make First and Last Name required or hidden. If you want users to must enter their First name when they sign up for your mailing list then check Required Field box. After making your changes click Save Field.

## Adding bootstrap forms CSS to mailchimp signup form

Now we have deleted Last Name field from our form. After deleting Last Name field click on Sign Up forms again and go to Naked tab and copy all HTML code to paste in your site.

Open your text editor such as [Sublimetext](https://www.sublimetext.com/), <a title="Adobe Brackets Review Great Free Text Editor from Adobe" href="http://www.tahirtaous.com/brackets-review/">Brackets</a> or any other Text editor you use, If you don't have any of these text editor then  open simple Notepad and paste all code there. Now find following lines of code.

{% highlight HTML %}
<div class="mc-field-group">
  <label for="mce-EMAIL">Email Address  <span class="asterisk">*</span>
</label>
  <input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
</div>

<div class="mc-field-group">
  <label for="mce-FNAME">First Name </label>
  <input type="text" value="" name="FNAME" class="" id="mce-FNAME">
</div>
{% endhighlight %}

This is HTML mark up for First Name and Last Name fields. We need to add some essential classes from Bootstrap framework to make this form elegant. because this is naked from with out any styling.

Now replace <code>mc-field-group</code> with <code>mc-field-group form-group</code>, i have just added <code>form-group</code> class from Bootstrap framework. Next find <code>class="required email"</code> in email input field and add one additional <code>form-control</code> class from bootstrap.

After adding new form-control class your you will have three classes <code>class="required email form-control"</code> for email input field.

Under First name label you can see input field for First name with blank CSS class <code>class=""</code>. just Add form-control class here.

You can also provide placeholder text for First name and Email field if you want. I have provided placeholder text for both input fields as well as you can see in code below.

{% highlight HTML %}
 <div class="mc-field-group form-group">
  <label for="mce-EMAIL">Email Address  <span class="asterisk">*</span>
 </label>
  <input type="email" value="" name="EMAIL" class="required email form-control" id="mce-EMAIL" placeholder="Type your email"> 
 </div>
 <div class="mc-field-group form-group">
  <label for="mce-FNAME">First Name </label>
  <input type="text" value="" name="FNAME" class="form-control" id="mce-FNAME" placeholder="Type your Name">
 </div>
{% endhighlight %}

Styling for First name and email field is complete. Now We are going to style submit button. Find following line

{% highlight HTML %}
 <input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button">
{% endhighlight %}

and add add new classes <code>btn btn-danger btn-lg</code> from bootstrap to style submit button.

If you want to change text for Subscribe button change value="Subscribe" to your new text e.g. value="Send Me Free Stuff".

{% highlight HTML %}
 <input type="submit" value="Send Me Free Stuff" name="subscribe" id="mc-embedded-subscribe" class="button btn btn-danger btn-lg">
{% endhighlight %}

### Result

Here you can see live preview of out final form.


<div class="mc-field-group form-group">
  <label for="mce-EMAIL">Email Address  <span class="asterisk">*</span>
</label>
  <input type="email" value="" name="EMAIL" class="required email form-control" id="mce-EMAIL" placeholder="Type your email">
</div>
<div class="mc-field-group form-group">
  <label for="mce-FNAME">First Name </label>
  <input type="text" value="" name="FNAME" class="form-control" id="mce-FNAME" placeholder="Type your Name">
</div>

<input type="submit" value="Send Me Free Stuff" name="subscribe" id="mc-embedded-subscribe" class="button btn btn-danger btn-lg">

That's all. Now copy your new edited mark up and add this to your website.

If you are using [WordPress](http://justlearnwp.com/create-a-wordpress-website/), To add widget to your WordPress website, Go to <code>Appearance > Widget > Select Text Widget</code> and paste your mark mark up there. Save widget and view front end of your website.

WordPress is a free Content Management System to create websites and blogs. You can create [30+ websites with WordPress](http://justlearnwp.com/create-a-wordpress-website/).

Starting a blog is also simple and easy. Read this step by step tutorial to learn [how to create a blog with WordPress](http://justlearnwp.com/how-to-create-a-blog/)

### Note

Remember you must be using Bootstrap based theme on your blog to see styles from bootstrap, if you are using any other theme which does not use Bootstrap you won't see any styling.