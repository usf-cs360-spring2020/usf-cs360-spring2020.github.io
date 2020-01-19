---
title: Midterm Website
navbar: Guides
layout: guides
key: 1.2
bump: true

assignments:
  - text: 'Midterm Alpha Release'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908099'

  - text: 'Midterm Beta Release'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908101'

  - text: 'Midterm Final Release'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908145'

blurb: |
  <p>Instead of a midterm exam, all students must complete a midterm group project. The primarily deliverable of the project is the project website, which is created incrementally in alpha, beta, and final releases.</p>
---

<style>
ul.task-list li.task-list-item {
  list-style-type: none;
}

ul.task-list li.task-list-item input.task-list-item-checkbox {
  margin: 0 .3em .25em -1.7em;
  vertical-align: middle;
}
</style>

## Content

The midterm website must contain the following pages and information:

| Web Page       | Page Type  | Release |
|:---------------|:-----------|:--------|
| Home/Landing   | Shared     | Alpha   |
| Team/About     | Shared     | Alpha   |
| Dataset        | Shared     | Alpha   |
| Prototypes     | Per Person | Beta    |
| Visualizations | Per Person | Final   |
{: style="width: auto;" class="table" }

Some pages will be shared across the entire group (e.g. home and team pages), whereas some pages will be per group member (e.g. prototype and visualization pages). Details on what each page should include are provided below.

## Setup

The website repository will be created using [Github Classroom](https://classroom.github.com/) and hosted using [Github Pages](https://pages.github.com/). We will setup these repositories during class as part of a lab assignment. Once created, the Github repository will be located at:

<input class="input tt" type="text" value="https://github.com/usf-cs360-spring2020/midterm-groupname/">

The associated Github Pages website will be located at:

<input class="input tt" type="text" value="https://usf-cs360-spring2020.github.io/midterm-groupname/">

In both, replace `groupname` with your midterm group name.

## Releases

Each group will have to create multiple [releases](https://help.github.com/articles/about-releases/) of their website. These releases act as checkpoints in the development of your projects and is a recommended process for any software project. It also allows us to grade a specific version of the project website without preventing groups from continuing development during the grading period.

Follow the [creating releases](https://help.github.com/articles/creating-releases/) guide on Github for exact steps on how to create a new release. The release version should follow this pattern:

| Release | Version | Examples |
|:--------|:-------:|:---------|
| Alpha Release(s) | `v0.1.#` | `v0.1.0`, `v0.1.1`, and so on... |
| Beta Release(s)  | `v0.2.#` | `v0.2.0`, `v0.2.1`, and so on... |
| Final Release(s) | `v1.0.#` | `v1.0.0`, `v1.0.1`, and so on... |
{: style="width: auto;" class="table" }

It is only necessary to create multiple releases if changes were made before the deadline that should be included in the grade. For example, suppose a group creates alpha release `v0.1.0` but discovers a typo before the deadline. That group can create a new alpha release `v0.1.1` and resubmit the link in Canvas.

Made a mistake? DO NOT DELETE RELEASES. Just [edit the release](https://help.github.com/articles/editing-and-deleting-releases/) or create a new release instead.

#### Alpha Release

The alpha release of your website must have draft content for all of the group pages. Specifically:

  - **Home Page:** Include a home/landing page with the following:

      - [ ] The **overall narrative**, goal, story, or theme of the project. Each visualization might have its own individual goal, but it must be relevant to the overall narrative stated here.

      - [ ] A **clear navigation** component to all of the other required content (e.g. navbar, menu).

      - [ ] The **proper attribution** (preferably in a footer) for any images, media, designs, templates, web frameworks, etc. used by the website.

  - **Team/About:** Include a page that describes [your group](midterm-project.html#midterm-groups). This should include:

      - [ ] Team **names**, including at least first name or nickname, optionally last name.

      - [ ] Team **profile photos** (should be professional, but can still be fun).

      - [ ] Team **biographies**, including major/minor, expected graduation year, and optionally a personal tidbit.

      - [ ] Team **contact information**, optionally including links to social media (Github, Linkedin, etc.).

      - [ ] Team **responsibilities**, indicating who worked on what. This includes who worked on which visualizations, and which team member(s) worked on the website design and shared content pages.

  - **Dataset:** Include a page that describes the [original dataset](midterm-project.html#dataset), dataset license, and shared processing/wrangling done to that data. Specifically:

      - [ ] **Proper attribution** for the original dataset. You will need to look at the original dataset page for how to give proper attribution. (This should include a link to the original data!*

      - [ ] The **dataset license** for the original dataset.

      - [ ] The **dataset size** (number of columns and rows).

      - [ ] The **relevant columns** from the original dataset, giving descriptions with the data types, possible values for categorical data, or the range of values (and possibly other simple statistics) for numerical columns.

      - [ ] Any **shared processing or filtering** done to the original dataset. Include enough detail that this process is repeatable by someone starting with the original dataset. If possible, link directly to the processed version of the data.

These are drafts; the content is expected to change over time. However, the drafts are still expected to have high quality. Check for spelling errors, typos, and grammar. Consider utilizing the [Writing Center](https://myusf.usfca.edu/lwsc/writing-center) if you are worried about your text.

The website layout and general design is *not* expected to change drastically between releases. This is your opportunity to stabilize on the website design so you can focus on the visualizations in future releases.

Submit a link directly to your release on Github in the [Midterm Alpha Release](https://usfca.instructure.com/courses/1590235/assignments/6908099) assignment on Canvas. Make sure you are submitting the correct link!

#### Beta Release

Update any of the content created for the alpha release as necessary, and add the following additional content:

  - **Prototypes:** Include a prototype page per person with the following:

      - [ ] A **multi-component visualization prototype** created using Tableau Desktop, [Vega-Lite](https://vega.github.io/vega-lite/), or another visualization prototyping tool. (Other tools must be pre-approved on Piazza.) The prototypes can be static or interactive.

      - [ ] Any **processing or wrangling** you had to do to the data for the prototype.

      - [ ] The **planned interactivity** you will implement in the final version.

      - [ ] How your prototypes **supports the theme** of the group project.

    Need inspiration? Check out a [Data Sketches](http://www.datasketch.es/february/) writeup; they discuss and demonstrate the process (including inspirations and discarded ideas) of creating their visualizations.

The prototypes you create for this release will be used as part of the [Midterm Feedback](midterm-feedback.html) process. While you should not modify the prototypes, you are expected to make modifications for the final version based on the feedback you received.

Submit a link directly to your release on Github in the [Midterm Beta Release](https://usfca.instructure.com/courses/1590235/assignments/6908101) assignment on Canvas. Make sure you are submitting the correct link!

#### Final Release

Update any of the content created for the beta release as necessary, and add the following additional content:

  - **Prototypes:** Update each prototype page with the following information (but do not modify the original prototype):

      - [ ] The **peer feedback** you received and how this impacted the final version of your visualizations.

  - **Visualizations:** Include one multi-component interactive visualization page per group member. The page should include:

    - [ ] A **multi-component interactive visualization** using [D3.js](https://d3js.org/) version 5 (using older versions will not receive full credit). See the [Visualizations](#visualizations) section for details.

    - [ ] The **data encoding** and how to interpret your visualization(s).

    - [ ] Instructions on **how to interact** with your visualization(s).

    - [ ] One or two **findings** that can be learned from your visualization(s) and how that **supports the theme** of the group project.

    - [ ] Any **inspirations** for your visualization(s) (including both design and functionality).

Submit a link directly to your release on Github in the [Midterm Final Release (Group)](https://usfca.instructure.com/courses/1590235/assignments/6908145) assignment on Canvas. Make sure you are submitting the correct link!



<!-- enables all the checkboxes -->
<script>
var checkboxes = document.getElementsByClassName("task-list-item-checkbox");

for (var i = 0 ; i < checkboxes.length ; i++) {
  checkboxes[i].disabled = false;
}
</script>
