---
title: Learning HTML, CSS, and JavaScript
navbar: Guides
layout: guides
key: 1.2
---

This guide provides some resources for getting started with the languages we will be using for web development in class. This includes: HTML, CSS, SVG, JavaScript, and JSON.

**Table of Contents**
{: .heading .has-text-grey }

[Web Technologies](#web-technologies)  
[Resources](#resources)  
[References](#references)  
[Remote Hosting](#remote-hosting)  
[Local Development](#local-development)

## Web Technologies

The core of basic web development starts with [**<u>H</u>yper<u>T</u>ext <u>M</u>arkup <u>L</u>anguage**](https://developer.mozilla.org/en-US/docs/Web/HTML)  (HTML). Briefly, **HTML** is a **markup language** that provides the content and structure of that content on a web page (e.g. titles versus paragraphs). A _markup language_ like HTML only annotates content and does not perform complex actions like a programming language might; instead all of the complexity is embedded in the browser that renders the HTML web page. We will use HTML v5 in class.

Whereas HTML provides the content of a web page, [**<u>C</u>ascading <u>S</u>tyle <u>S</u>heets**](https://developer.mozilla.org/en-US/docs/Web/CSS) (CSS) provides the visual style of that content (e.g font style and colors). A web page can be created in HTML only, but nearly all modern web pages utilize both HTML and CSS. We will also use [CSS selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors) to both style and access content in our visualizations. We will use CSS v3 in class.

When it comes to creating graphics on web pages, we will use [**<u>S</u>calable <u>V</u>ector <u>G</u>raphics**](https://developer.mozilla.org/en-US/docs/Web/SVG) (SVG). SVG is another text-based markup language, but instead of providing text content it provides scalable graphic content instead (i.e. a circle or line). We can also use CSS to style SVG content.

While HTML, SVG, and CSS are great for static web content, the restriction of being markup versus full-fledged programming languages means it cannot be used for dynamic content. That is where the [**JavaScript**](https://developer.mozilla.org/en-US/docs/Web/JavaScript) (JS) programming language comes in. As described by [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript), JavaScript is "a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles."

Confused? You are not alone! Many programmers struggle when they first encounter JavaScript, especially if they are unfamiliar with asynchronous declarative or functional programming. There are a few things to keep in mind: it is *not* based on Java syntax (the name is misleading), it has its own notion of [truthy](https://developer.mozilla.org/en-US/docs/Glossary/Truthy) values and [sameness versus equality](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness), and its a very powerful programming language capable of supporting the most complex of web applications. Thankfully, we will only use *basic* JavaScript in this class (sometimes called *vanilla* JavaScript).

We will use JavaScript primarily alongside the [**<u>D</u>ata-<u>D</u>riven <u>D</u>ocuments**](https://d3js.org/) (D3 or D3.js) JavaScript library to create interactive, web-based visualizations driven by data.

It is possible to have HTML, CSS, SVG, and JavaScript all in a single HTML file. It is also possible to break these up into separate files: `.htm` or `.html` files for HTML, `.css` files for CSS, `.svg`  files for SVG, and `.js` files for JavaScript.

## Resources

There is a great set of beginner to advanced guides for all of these web technologies on the [**Mozilla Developer Network**](https://developer.mozilla.org/en-US/) (MDN). I recommend starting here:

  - [Web technology for developers](https://developer.mozilla.org/en-US/docs/Web)
  - [Getting started with the Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)

Even if you are familiar with these technologies, you may want to review some specific topics:

  - [Using CSS selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors)
  - [Equality comparisons and sameness](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness)
  - [Working with JSON](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON)
  - [General asynchronous programming concepts](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Concepts)
  - [Functions: Constructor vs. declaration vs. expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions#Constructor_vs._declaration_vs._expression)

Here are a few other resources that may be useful for learning HTML, CSS and JavaScript:

  - [Introduction to HTML](https://lab.github.com/githubtraining/introduction-to-html) (Github Training Course)
  - [Introduction to HTML](https://beta.observablehq.com/@mbostock/introduction-to-html) (Observable Notebook)
  - [Introduction to HTML](https://www.codecademy.com/learn/learn-html) (Codecademy)
  - [Introduction to Basic HTML and HTML5](https://learn.freecodecamp.org/responsive-web-design/basic-html-and-html5/) (freeCodeCamp)
  - [Introduction to CSS](https://learn.freecodecamp.org/responsive-web-design/basic-css/) (freeCodeCamp)
  - [Introductionto JavaScript](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript/) (freeCodeCamp)
  - [Introduction to JavaScript](https://www.codecademy.com/learn/introduction-to-javascript) (Codecademy)
  - [JavaScript](https://en.wikibooks.org/wiki/JavaScript) (Wikibooks)
  - [JavaScript for Cats](http://jsforcats.com/)

You also have access to [**Linkedin Learning**](hhttps://myusf.usfca.edu/ets/educational-technologies/linkedin) which has several free short online courses available on all of these web technologies. There are many more options that can be found with a web search, especially if you prefer videos over text.

## References

The resources listed above are great for learning these web technologies, but sometimes you just need to know the valid syntax for something. My favorite set of references for this purpose are the [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/) references.

- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [SVG](https://developer.mozilla.org/en-US/docs/Web/SVG)
- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [JSON](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON)

## Remote Hosting

Small examples may be hosted via a combination of [Github gists](https://gist.github.com/), [bl.ocks.org](https://bl.ocks.org/), [blockbuilder.org](https://blockbuilder.org/), and [vizhub.com](https://vizhub.com/).

The files required for the visualization(s) are stored in a [gists](https://gist.github.com/), which is basically a lightweight `git` repository meant for sharing code with others. This should include an `index.html` file, and any other files and resources required by the code. See the [Github Help](https://help.github.com/categories/gists/) pages for more information about gists.

To view the visualization, load the gist in [bl.ocks.org](https://bl.ocks.org/). See the [About](https://bl.ocks.org/-/about) page for how to view a gist on [bl.ocks.org](https://bl.ocks.org/). Keep in mind there is sometimes a slight delay between the files cached by [bl.ocks.org](https://bl.ocks.org/) and those hosted on [gist.github.com](https://gist.github.com/). If you want to modify the code and see live changes, load the gist in [blockbuilder.org](https://blockbuilder.org/) instead.

These websites use the `gistid` in the URL, with the primary difference being the domain:

```
https://gist.github.com/username/gistid
https://bl.ocks.org/username/gistid
https://blockbuilder.org/username/gistid
```

You can also use [vizhub.com](https://vizhub.com/) as an alternative to [blockbuilder.org](https://blockbuilder.org/). Small examples may also be hosted using [Observable Notebooks](http://beta.observablehq.com/) as well. See the [Introduction to D3.js](https://beta.observablehq.com/d/28ba93f58fb82f49) Observable notebook for more.

For hosting an entire website of visualizations, use [Github Pages](https://pages.github.com/). There are many guides for setting up Github repositories for Github Pages:

  - [Github Pages](https://pages.github.com/) (Landing Page)
  - [Github Pages](https://lab.github.com/githubtraining/github-pages) (Github Training Course)
  - [Github Pages Basics](https://help.github.com/categories/github-pages-basics) (Github Help Pages)
  - [Getting Started with GitHub Pages](https://guides.github.com/features/pages/) (Github Guides)
  - [Customizing Github Pages](https://help.github.com/categories/customizing-github-pages) (Github Help Pages)

The [course website](https://github.com/usf-cs360-spring2020/usf-cs360-spring2020.github.io) is also hosted using Github Pages.

## Local Development

You cannot simply open up an HTML file in a browser when it comes to dynamic content. Instead, run a local web server to run and debug visualizations locally. This is especially important for loading data. There are many options for running a local web server.

The official [D3 wiki](https://github.com/d3/d3/wiki#local-development) recommends using `npm` to run the [`http-server`](https://www.npmjs.com/package/http-server) package from [Node](https://nodejs.org/en/):

```
npm install -g http-server
http-server &
```

It is also possible to [use Python to run a web server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server#Running_a_simple_local_HTTP_server). Use the [SimpleHTTPServer](https://docs.python.org/2/library/simplehttpserver.html) module if Python version 2 is installed:

```
python -m SimpleHTTPServer
```

Use the [http.server](https://docs.python.org/3/library/http.server.html) module for Python version 3:

```
python3 -m http.server
```

Another option is to develop in [Atom](https://atom.io/) and use the [live-server](https://atom.io/packages/atom-live-server) package to launch a local web server.

For all of these options, run the local web server from the same directory as the `index.html` file. Access the website at `http://localhost:[port]` where `[port]` is the port number used by the web server. This is usually something like `3000`, `4000`, or `8080`.
