---
layout: post
title: "CSS Box Model"
---

### The Box Model

The Box Model is something that describes how all of these boxes behave, and how the browser knows about the space they occupy on a page.

We’ve told you that you can specify width, height and borders, but there’s more than that. You can also specify a `padding`, which is some space between your content and the edge of the box. And you can specify a `margin`, which is the size between the box and it's neighboring boxes.

Here you can see how these different properties compose a box:

<figure>
  <img src="{{site.baseurl}}/assets/images/box-model.png" alt="A visualization of the box model.">
  <figcaption>
    <p>A visualization of the box model.</p>
  </figcaption>
</figure>

Now, how much space does this box occupy on a page? We need to take into account not just the width and the height that was specified, but also the paddings and the borders (we can forget about the margins for now). So in reality, our box occupies a width of 80px plus 5px on each side for the paddings, plus 1px for each border (note we're using the border shorthand). So that means that the real width is 92px.

Now apply some spacing to the elements on your page!
