---
title: Homework 1
navbar: Guides
layout: guides
key: 2.1
bump: true

tags:
  - text: 'Pending'
    type: 'is-primary'

assignments:
  - text: 'Homework 1 Functionality'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6907999'

  - text: 'Homework 1 Peer Review Submission'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908002'

  - text: 'Homework 1 Peer Review Feedback'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908004'

blurb: |
  <p>For this homework assignment, you must visualize the <a href="https://data.sfgov.org/Transportation/Air-Traffic-Passenger-Statistics/rkru-6vcg">Air Traffic Passenger Statistics</a> dataset with basic visualization techniques using <a href="https://www.tableau.com/products/desktop">Tableau Desktop</a> and <a href="https://d3js.org/">D3.js</a> (version 5).</p>
---

## Dataset

Visualize the [Air Traffic Passenger Statistics](https://data.sfgov.org/Transportation/Air-Traffic-Passenger-Statistics/rkru-6vcg) dataset from [DataSF](https://datasf.org/opendata/).

The original dataset includes over 21.k rows as of December 2019. Filter this down to a reasonable size for each individual visualization!

The original dataset includes 12 columns. Most of these columns are categorical text, such as the operating airline and geographic region. The activity period is encoded as a number but may be wrangled to be interpreted as a date. The only other number is passenger count. Read the provided data dictionary prior to any data wrangling or visualization!

## Requirements

Create one image or SVG per visualization. Visualizations may be placed on the same page or separate webpages. Regardless, the homework website must have clear navigation to each of the visualizations.

Generally, each image should not exceed 960 pixels by 500 pixels in size. Some exceptions are reasonable. For example, a small multiples visualization may exceed this size as long as each individual multiple remains within those size requirements. It may also be appropriate to exceed the height requirement for horizontal bar charts.

### Functionality

The letter grade for this homework will be broken down as follows:

| Letter | Requirement |
|:------:|:------------|
| D | Prototype **3** unique visualizations using Tableau Desktop. |
| C | D-level requirements plus implement **1** of the Tableau prototypes in D3 version 5. |
| B | D-level requirements plus implement **2** of the Tableau prototypes in D3 version 5. |
| A | D-level requirements plus implement **3** of the Tableau prototypes in D3 version 5. |
{: .table .is-hoverable .is-auto }

See below for details on each grade level.

##### D-Level Functionality
{: .has-text-grey }

Prototype three different basic visualizations of the dataset using Tableau Desktop. Specifically:

  - Create at least **3 different visualizations**. This means you need 3 different "sheets" in Tableau and must export 3 different images to include on your website.

  - Use at least **2 different encodings** from the following list:
    - <i class="far fa-chart-scatter fa-li"></i> Encode data using points (e.g. scatter or bubble plot)
    - <i class="far fa-chart-bar fa-li"></i> Encode data using bars (e.g. horizontal/vertical bar charts, stacked or grouped bars, small multiples, and histograms)
    - <i class="far fa-chart-area fa-li"></i> Encode data using area (e.g. area charts, stacked area, small multiples)
    - <i class="far fa-chart-pie fa-li"></i> Encode data using heatmaps or pie charts
    {: .fa-ul }

  - Use at least **2 different perspectives** of the data.  This can be achieved by grouping, filtering, or aggregating the data differently. For example, one visualization can use data grouped by region and another uses data grouped by activity type instead.

  - Use **color to encode data** in *at least* one visualization. This visualization must include a color legend in the static image export.

  - Use **titles and axis labels** where appropriate to make sure the encoding is clear.

  - For each visualization, **include a caption** that includes your name and original data source.

Export your Tableau visualizations as **static images** and include them on your homework submission website under the "Prototypes" heading. None of the visualizations for this homework assignment need to be interactive.

Use the "Dashboards" feature in Tableau to make sure your images will fit within the size constraints and the legend and caption are clearly visible.

You must fully meet these requirements before moving on to the next grade level.

##### C-Level Functionality
{: .has-text-grey }

Implement one of the Tableau prototypes in D3 version 5. Specifically:

  - Use the same visualization technique and data encoding as one of your Tableau visualizations. <span class="tag is-primary">Required</span>

  - Match as much of the design from your Tableau prototype as possible. This includes colors for non-data elements, style of grid lines, tick labels, sort order, and so on. <span class="tag">Recommended</span>

  - Include the captions, titles, and legends found in your Tableau prototype in your D3 implementation. <span class="tag">Recommended</span>

You must fully meet these requirements before moving on to the next grade level.

##### B-Level Functionality
{: .has-text-grey }

This has the same requirements as the C-level functionality, except for a second Tableau prototype.

##### A-Level Functionality
{: .has-text-grey }

This has the same requirements as the B-level functionality, except for a third Tableau prototype.

### Writeups

The following writeups are required to earn credit, regardless of the level of functionality implemented:

  - About the original dataset, including its source, size, license, and when you accessed it.

  - Your self-assessment of the letter grade you should earn (D, C, B, or A). For each level, indicate whether you met the functionality requirements and how (if appropriate). *You do not need to indicate whether you should receive a plus or minus letter grade.*

  - Your professional information, including your name, photo, USF email address, major, expected graduation date, and brief bio about yourself.

For each visualization you create, you must also include the following writeups:

  - How to interpret your visualization, indicating how the data is encoded. For example, "passenger count is encoded by the length of the bar, so longer bars represent higher passenger count."

  - Any per-visualization data wrangling you performed on the original dataset, and how you wrangled the data (e.g. Tableau, Excel, using the website interface). Link to the wrangled data when possible.

  - One conclusion you can make about the data using your visualization. The conclusion should ideally be something that a simple statistic could not replace. For example, "airline X has the highest passenger count over this time period" is a simple conclusion that will meet this requirement, but may not earn a plus-level letter grade.

The writeups do not need to be long---often 1 paragraph with 3 to 5 sentences will suffice.

### Plus/Minus Grades

It is up to the discretion of the grader to assign a minus letter grade (e.g. B-), normal letter grade (e.g. B), or plus letter grade (e.g. B+). The following will be considered in making this determination:

  - Are the functionality requirements fully implemented and reasonably bug-free?

  - Are all of the relevant details provided with the visualizations (such as legends, titles, annotations)?

  - Are all of the required writeups (such as how to interpret your visualization) included?

  - Are the writeups reasonably well-written (with no misspellings and decent grammar).

  - Are the inspirations, sources, and references properly attributed?

  - Is the website well-designed and easy to navigate?

All of the above must be true to qualify for a plus-level letter grade.

## Hints

  - In Tableau, you can group together categories. Just click the categories you want to group, and select the paperclip icon to group them together. This will create a “Column Name (group)” dimension, and you can click that to edit the groupings and group names. This is especially helpful if there are many categories with very few items.

  - In Tableau, you can export the data specific to each worksheet. I recommend you use that data for each of your D3 visualizations to make things easier. For example, if you group by weekday in one of your Tableau worksheets, you can export a dataset grouped by weekday to use in your D3 visualization.

  - Keep in mind that showing data grouped by activity period may be misleading, since months do not have equal number of days. You can instead calculate an average or a ratio based on the number of days in the specific month.

  - The visualization should be your unique take on the dataset. However, there are a lot of D3 examples on the web that you are welcome to reference. Just be sure to properly cite your references and avoid copying/pasting large chunks of code without attribution.

  - DO NOT VISUALIZE THIS ON A MAP. We’ll get to map visualizations later.

  - DO NOT USE AN OLDER VERSION OF D3. If you are using an example as inspiration, avoid any examples using D3 version 3, which is *significantly* different from version 5. However, version 4 and 5 are similar. The primary difference is how you load files. See the [Change Log](https://github.com/d3/d3/blob/master/CHANGES.md) for details.
