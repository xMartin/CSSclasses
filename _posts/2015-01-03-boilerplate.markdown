---
layout: post
title: "Boilerplate"
---

### Elements and Tags
Elements and Tags are the building blocks of HTML.

Elements are what makes up a HTML document. You can put elements inside of other elements. An element can include three things: a tag, attributes, and content.

A Tag is the thing that indicates an element’s purpose. For example, the `<p>` tag indicates a paragraph of text is in that element, and the `<li>` represents a ‘list item’. You’ll notice they’re always surrounded by angle brackets. Opening and Closing tags mark the beginning and end of an element and wrap its content, like so:

{% highlight HTML %}
<p>This is a paragraph.</p>
{% endhighlight %}

You can see the closing tag includes a `/` before its name; otherwise it would be another opening tag!

Always double-check that you’ve closed all your elements; otherwise, a browser can and will get mixed up trying to understand your HTML document.

Lastly, having elements inside of each other (“nesting”) looks just like this:

{% highlight HTML %}
<p>This is a sentence, with an <em>em</em> element ("emphasize") inside of it.</p>
{% endhighlight %}

or this:

{% highlight HTML %}
<div class="main-container">
  <h1>The h1 tag indicates the primary header of the document.</h1>
  <p>Some text.</p>
</div>
{% endhighlight %}

In the above example, you can see our first case of an attribute. It starts with a lowercase name, and then is almost always followed by an = and a ‘value’ that’s surrounded in double quotes, "like this". An element can have many attributes, in which case you separate them by spaces, as you’ll see soon. Attributes give information about an element in particular.


## Add web page content

Let's start adding some HTML and content to out `index.html` page.
First off our name and a short summary.

1. Open `index.html` in the editor.
1. Copy & paste the following code:


```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1>My Name</h1>
    <h2>Summary</h2>
    <p>About me...</p>
  </body>
</html>
```

1. Replace `My Name` with your name and also `About me...` with a sentence describing yourself
1. Save the changes
1. Switch back to your web browser and refresh the page

Your name and summary are now visible 🤘

Let's now add a list of interests.

1. Copy the following code and paste underneath the content we just added

```html
<h2>Interests</h2>
<li>Interest...</li>
<li>Interest...</li>
<li>Interest...</li>
```

Our updated HTML should looks something like:

```html
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <h1>My Name</h1>
    <h2>Summary</h2>
    <p>About me...</p>
    <h2>Interests</h2>
    <li>Interest...</li>
    <li>Interest...</li>
    <li>Interest...</li>
  </body>
</html>
```

1. Replace each `Interest...` text with an interest of your own
1. Save the changes
1. Switch back to your web browser and refresh the page

Your interests are now visible 🤘
