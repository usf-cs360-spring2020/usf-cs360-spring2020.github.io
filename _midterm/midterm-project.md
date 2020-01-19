---
title: Midterm Project
navbar: Guides
layout: guides
key: 1.1

assignments:
  - text: 'Midterm Group'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908097'

  - text: 'Midterm Website'
    link: 'midterm-website.html'

  - text: 'Midterm Feedback'
    link: 'midterm-feedback.html'

  - text: 'Midterm Presentation'
    link: 'midterm-presentation.html'

blurb: |
  <p>Instead of a midterm exam, all students must complete a midterm group project. This guide details all of the associated requirements for this project.</p>
---

## Groups

The midterm project *must* be completed in a group. Midterm groups should ideally be 3 students from the same section. There is a maximum of 10 groups total. Groups of 2 or 4 will be approved only when other options not available.

To form and submit your midterm group, see the [Midterm Group](https://usfca.instructure.com/courses/1590235/assignments/6908097) assignment on Canvas.

## Grading

There will be two scores assigned for the midterm project: a [group score](https://usfca.instructure.com/courses/1590235/assignments/6908145) worth 50 points and an [individual score](https://usfca.instructure.com/courses/1590235/assignments/6908144) worth 150 points. The amount of work required for the midterm project will depend on the number of people in the group. This includes the required number of visualizations and the length of presentation time.

Unlike the homework and lab assignments, projects will be graded on their functionality *and* design. This includes the functionality and design of the overall website, text, and visualizations.

The instructor will grade the final release of the midterm project websites. The midterm group project will be graded not just on whether you meet the core requirements, but also how well you meet or exceed those requirements. Specifically:

| Letter | Description |
|:------:|:------------|
| F | Reserved for projects that do not meet the minimum requirements. |
| D | Reserved for projects that meet the minimum requirements, but fail to deliver informative visualizations and a professional website. |
| C | Reserved for those projects that meet the minimum requirements, and deliver informative visualizations and a professional website. |
| B | Reserved for those projects that *exceed* the minimum requirements, and deliver informative visualizations and a professional website. |
| A | Reserved only for those projects that go *above and beyond* the minimum requirements, and deliver a *highly* effective visualizations and a well-written professional website. |

While code quality will not be assessed, students are still expected to adhere to the honor code. Claiming work (either code, data, or design) that is not yours or failing to provide proper attribution can result in an automatic F letter grade.

Each intermediate project assignment will have a rubric posted for determining the grade.

## Dataset

All groups must visualize the following dataset:

  - [SF Fire Department Calls for Service](https://data.sfgov.org/Public-Safety/Fire-Department-Calls-for-Service/nuek-vuh3)
  {: style="list-style-type: none;"}

Students must familiarize themselves with this dataset. Make sure to read the data dictionary and read the [About Us](https://sf-fire.org/about-us) page of the San Francisco Fire Department. Groups are also welcome to find related datasets to the one above that can help augment their visualizations as well.

Each group must decide on a subset (or multiple subsets) of this dataset that will be manageable in size. There is no exact size requirement; the subset must be big enough to warrant several unique visualizations but not too large to load in the browser or Tableau Desktop.

The subset can be selected by focusing on specific categories or aggregating the data. However, it should support an **cohesive theme** that the entire group will integrate into their individual visualizations. See the [Theme](#theme) section for details.

## Theme

Each group must determine a **cohesive theme** for the project. This could be an overall story that each visualization will help tell, or a broad question that each visualization will help answer in different ways.

Group communication and coordination will be key. While each visualization page will be worked on individually, the visualizations should complement each other and support the theme. The group project score will consider how cohesive the theme is across the entire project, and the individual project score will consider how well the visualization(s) support the theme.

Beyond having a cohesive story or question, the encodings and styles should also be kept as consistent as possible across visualizations. For example, use the same color encoding for categories throughout the entire project.

## Visualizations

Each group must produce *at least* one unique interactive multi-component visualization page per person using [D3.js](https://d3js.org/) version 5 (using older versions will not receive full credit). Visualizations should be both informative and aesthetically pleasing. The individual components on the visualization page should have their interactivity linked. For example, highlighting a category in one component should highlight that same category in all components.

Keep the required screen space to view your visualizations within 1440 x 900 pixels. These are maximums; your visualizations do not need to take up that entire space and do not need to have that aspect ratio. Your visualizations do not need to be responsive to the browser size.

The visualization techniques can include any of the basic, time series, or multivariate data visualization techniques we have discussed thus far in class. This includes: <i class="fas fa-table"></i> **tables** (normal or Bertin-style), <i class="fas fa-grip-horizontal"></i> **heatmaps** (rectangular or circular), <i class="fas fa-chart-bar"></i> **bar charts** (normal, grouped, stacked, 100% stacked, horizontal or vertical, small multiples), <i class="fas fa-chart-line"></i> **line charts** (normal, multi-series, small multiple, slope graphs, rectangular or circular, small multiples), <i class="fas fa-chart-area"></i> **area charts** (normal, stacked, 100% stacked, small multiples, **streamgraphs**, rectangular or circular, **horizon charts**, joyplots), <i class="fas fa-chart-pie"></i> **pie charts** (normal, small multiples, ~~donut charts~~), <i class="fas fa-chart-scatter"></i> **scatterplots** (normal, hexbinning, bubble charts, scatterplot matrices), **parallel coordinates** (rectangular or circular), or **distribution plots** (histograms, boxplots, violin plots, density plots, beeswarm plots, small multiples).

## Website

The primary deliverable for the midterm group project will be a public website using [Github Classroom](https://classroom.github.com/) and [Github Pages](https://pages.github.com/). This website will be created incrementally via alpha, beta, and final releases. Each release adds additional content to the website.

See the [Midterm Website](midterm-website.html) guide for more details.

## Feedback

Since project grades will be based on both functionality *and* design, receiving and responding to feedback is critical. Groups will switch between presenting their prototypes and providing peer feedback on week 7 (Tue 3/3 and Thu 3/5).

See the [Midterm Feedback](midterm-feedback.html) guide for more details.

## Presentation

Each group must present their midterm project in class on week 9 (Tuesday 3/17 and Thursday 3/19). The presentation length must be 5 minutes per person; a 3 person group must present for 15 minutes. The presentation dates will be semi-randomly assigned by the instructor (taking into account the size of groups and length of presentations).

See the [Midterm Presentation](midterm-presentation.html) guide for more details.
