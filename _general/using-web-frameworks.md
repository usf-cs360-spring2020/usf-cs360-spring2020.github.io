---
title: Using Web Frameworks
navbar: Guides
layout: guides
key: 1.3
---

If you have a strong understanding of HTML and CSS, I encourage you to explore using various different modern front-end web frameworks for your homework and project websites.

*Imagine how great it will be to show off a modern responsive website with interactive visualizations and open source code to potential employers!*

I do *not* recommend exploring heavy-duty web application frameworks like [React](https://reactjs.org/), [Angular](https://angularjs.org/), or [Vue](https://vuejs.org/). While widely used and powerful, those frameworks will be overkill for class. However, if you are interested in front-end programming, I recommend looking into them at some point.

Instead, I recommend CSS-only or CSS with minimal JavaScript front-end frameworks that help you build responsive (i.e. changes layout for mobile devices) and modern websites. These frameworks come with built-in CSS classes that help with style and layout.

### Getting Started

Using a front-end CSS framework *will* increase the amount of HTML code you must write. There are many classes that must be combined together to create responsive mobile-ready layouts.

Take for example these columns:

<div class="columns">
  <div class="column">
    <p class="is-primary notification">First</p>
  </div>

  <div class="column">
    <p class="is-info notification">Second</p>
  </div>

  <div class="column">
    <p class="is-success notification">Third</p>
  </div>
</div>

Change the size of the browser to see how those columns react. Using Bulma, that requires combining `div` elements and the `column` class to generate:

```html
<div class="columns">
  <div class="column">
    <p class="is-primary notification">First</p>
  </div>

  <div class="column">
    <p class="is-info notification">Second</p>
  </div>

  <div class="column">
    <p class="is-success notification">Third</p>
  </div>
</div>
```

It can take time to learn how to apply the different CSS classes, but once you have a working layout it is relatively easy to plug in content using the same layout over and over again. (That is close to what I do for class websites.)

Each framework has a boiler-plate template you can start with and plug in your own content. Here is one I created for this class using Bulma:

  - Pending
  {: style="list-style-type: none;"}

You are welcome to use it for your homework and projects.

### CSS Frameworks

Some example CSS frameworks include:

- [Bulma](https://bulma.io/) (Used by [this website](/).)

- [Bootstrap](https://getbootstrap.com/) (Originally from Twitter. Used by my [personal website](https://sjengle.cs.usfca.edu/).)

- [Pure.css](https://purecss.io/) (Originally from Yahoo.)

- [Material](https://material.io/develop/web/) (Originally from Google.)

- [Semantic UI](https://semantic-ui.com/)

Search for "CSS framework" to find many other alternatives. Some include JavaScript components as well. Be careful about choosing a framework that relies too heavily on JavaScript---we do not want our JavaScript visualizations to compete for resources.


<style>
.notification {
  padding: .75rem !important;
  font-size: 0.75rem;
}
</style>

You may not want to use my websites as a starting point. In addition to using the Bulma or Bootstrap frameworks, I also use [Jekyll](https://jekyllrb.com/) to generate the static web pages from different templates.
{: .notification }
