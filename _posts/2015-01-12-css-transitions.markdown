---
layout: post
title: "CSS Transitions"
---

### Transition
Transitions are a nice way to add some interactive animations to your site. If you add a transition to an element, the browser will automatically animate between two states when they change. To try that you can combine what you just learned about classes and `:hover` and add the `transition` property to the mix:

{% highlight HTML %}
<head>
<!-- ... -->
  <style>
    .changeonhover {
      color: white;
      background-color: green;
      text-align: center;
      width: 300px;
      height: 200px;
      font-family: sans-serif;
      border: 5px solid black;
      transition: 1s all;
    }
    .changeonhover:hover {
      background-color: blue;
      width: 600px;
      height: 300px;
    }
  </style>
</head>
<body>
  <div class="changeonhover">Hover me! Hover Me!</div>
</body>
{% endhighlight %}

Notice how you did not need to define an animation but still the browser animates between the two states? All we did is insert `transition: 1s all;` which is the transition shorthand with just the first two values that are a `transition-duration` of 1 second and the `transition-property` of `all` which means the browser will animate between all properties that have changed.
