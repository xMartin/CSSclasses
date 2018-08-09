---
layout: post
title: "CSS Class Selector"
---

### Class Selector
Until now we used the element selector to apply styles to an element. What’s wrong with that? Nothing, until you want to have two or more differently styled `p`s on your page.

{% highlight HTML %}
<head>
<!-- ... -->
  <style>
    p {
      color: white;
      background-color: green;
      width: 300px;
      height: 200px;
    }
  </style>
</head>
<body>
  ...
  <p>About me...</p>
  <p>I am a different paragraph but i look like the other one! 😞</p>
</body>
{% endhighlight %}

Copy this code example into your html file, and check out what it looks like in the browser. Now let’s say the second `p` should be blue. We can achieve that by assigning classes to the `p`s in our HTML. We can then apply styles to each class in our CSS:

{% highlight HTML %}
<head>
<!-- ... -->
  <style>
    p {
      color: white;
      background-color: green;
      width: 300px;
      height: 200px;
    }

    .greenthing { background-color: green; }

    .bluething {
      background-color: blue;
      font-family: serif;
      text-align: center;
    }

    .border-dotted { border: 5px dotted black; }
  </style>
</head>
<body>
  ...
  <p class="greenthing">About me...</div>
  <p class="bluething border-dotted">I am a different paragraph and i don't look like the other one any more! 😀</p>
  ...
</body>
{% endhighlight %}

Now here you should note several things. Both `p`s get the styles of the `p` rule, as this applies to all `p`s. Then the first `p` also gets the styles of the class `.greenthing`. In HTML the classes get assigned by writing a class attribute inside of the opening tag of the element. The second `p` has two classes – you can assign as many of them as you want! Just separate them by a space. In the CSS code, class selectors are marked by a dot like this: `.border-dotted`. This class is remarkable as it `overrides` the border style that was defined in the `p` selector.
