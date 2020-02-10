---
title: Homework 2
navbar: Guides
layout: guides
key: 2.2

tags:
  - text: 'Updated'
    type: 'is-primary'

assignments:
- text: 'Homework 2 Functionality'
  link: 'https://usfca.instructure.com/courses/1590235/assignments/6908005'

- text: 'Homework 2 Peer Review Submission'
  link: 'https://usfca.instructure.com/courses/1590235/assignments/6908006'

- text: 'Homework 2 Peer Review Feedback'
  link: 'https://usfca.instructure.com/courses/1590235/assignments/6908007'

blurb: |
  <p>For this homework assignment, you must visualize data from the "<a href="https://opportunityinsights.org/paper/mobilityreportcards/">Mobility Report Cards: The Role of Colleges in Intergenerational Mobility</a>" project using a multivariate visualization technique in D3.js (version 5).</p>
---

## Dataset

Visualize the "Baseline Cross-Sectional Estimates of Child and Parent Income Distributions by College" dataset from the "[Mobility Report Cards: The Role of Colleges in Intergenerational Mobility](https://opportunityinsights.org/paper/mobilityreportcards/)" project from [Opportunity Insights](https://opportunityinsights.org/).

Look at the supplemental material, especially the conclusions of the study, available on the website. Visualizations that conflict with the study conclusions may need close examination.

The exact dataset is the "Baseline Cross-Sectional Estimates of Child and Parent Income Distributions by College" dataset (also referred to as "Online Data Table 2"). The direct links are:

[mrc_table2.csv](https://opportunityinsights.org/wp-content/uploads/2018/04/mrc_table2.csv)  
[Codebook-MRC-Table-2.pdf](https://opportunityinsights.org/wp-content/uploads/2018/04/Codebook-MRC-Table-2.pdf)

Choose approximately 50 or more rows and at least 4 columns to focus on in this dataset. Visualizations may be supplemented by other datasets if appropriate to provide additional context.

## Requirements

Create one image or SVG per visualization. Visualizations may be placed on the same page or separate webpages. Regardless, the homework website must have clear navigation to each of the visualizations.

Each visualization should not exceed 960 pixels wide. Visualizations should not exceed 500 pixels in height, however some exceptions are reasonable. For example, it is appropriate to exceed the height requirement for some heatmaps or vertical parallel coordinates. A small multiples visualization may exceed this size as long as each individual multiple remains within those size requirements.

### Functionality

The letter grade for this homework will be broken down as follows:

| Letter | Requirement |
|:------:|:------------|
| `D` | Prototype and implement a bubble plot. |
| `C` | Prototype and implement a *normalized* heatmap. |
| `B` | Prototype and implement a small multiples visualization *-or-* both a bubble plot and heatmap. |
| `A` | Prototype and implement a parallel coordinates visualization -or- a scatterplot matrix (choose one). |

See below for details on each grade level.

##### D-Level Functionality
{: .has-text-grey }

Prototype a bubble chart in [Tableau Desktop](https://www.tableau.com/products/desktop) or [Vega Lite](https://vega.github.io/vega-lite/examples/#scatter--strip-plots) and then implement that visualization in [D3.js](https://d3js.org/) version 5.

The bubble chart must use horizontal position, vertical position, circle area, and circle color to encode at least 4 different columns from the dataset. The prototype and D3.js versions must use the exact same encodings, but may differ slightly in the style of the axes, tick marks, titles, labels, legend placement, and so on.

##### C-Level Functionality
{: .has-text-grey }

Prototype a *normalized* heatmap in [Tableau Desktop](https://www.tableau.com/products/desktop) or [Vega Lite](https://vega.github.io/vega-lite/examples/#table-based-plots) and then implement that visualization in [D3.js](https://d3js.org/) version 5.

Since the values across columns may have different scales (e.g. percent female ranges from 0 to 1 but parent median income ranges from 21,200 to 226,700), you need to normalize the values in each column. There are different forms of normalization; use [feature scaling](https://en.wikipedia.org/wiki/Feature_scaling) on each column before visualizing on the heatmap.

The prototype and D3.js versions must use the exact same encodings, but may differ slightly in the style of the axes, tick marks, titles, labels, legend placement, and so on.

##### B-Level Functionality
{: .has-text-grey }

There are two options for this grade level. Choose exactly 1 option.

  1. Prototype a small multiples visualization using an basic visualization technique (such as small multiple line charts, small multiple bar charts, etc.) in [Tableau Desktop](https://www.tableau.com/products/desktop) or [Vega Lite](https://vega.github.io/vega-lite/examples/#faceting-trellis-plot--small-multiples) and then implement that visualization in [D3.js](https://d3js.org/) version 5.

      The prototype and D3.js versions must use the exact same encodings, but may differ slightly in the style of the axes, tick marks, titles, labels, legend placement, and so on. The layout does *not* need to match exactly since laying out multiples on a grid is harder in Tableau or Vega Lite.

  2. Prototype and implement both a bubble chart and *normalized* heatmap. See the D-level and C-level functionality sections for details (both must be completed).

If creating multiple visualizations and those visualizations share the same encodings, only one legend needs to be provided. For example, if both the bubble chart and heatmap utilize the same color scale, only one color legend is required.

##### A-Level Functionality
{: .has-text-grey }

There are two options for this grade level. Choose exactly 1 option.

  1. Prototype a scatterplot matrix in [Tableau Desktop](https://www.tableau.com/products/desktop) or [Vega Lite](https://vega.github.io/vega-lite/examples/interactive_splom.html) and then implement that visualization in [D3.js](https://d3js.org/) version 5.

      Recall that you need to visualize at least 4 columns from the dataset. The prototype and D3.js versions must use the exact same encodings, but may differ slightly in the style of the axes, tick marks, titles, labels, legend placement, and so on. The layout does *not* need to match exactly since modifying the diagonal or redundant triangle is harder in Tableau or Vega Lite.

  2. Prototype a parallel coordinates plot in [RAWGraphs](http://app.rawgraphs.io/) or [Vega Lite](https://vega.github.io/vega-lite/examples/parallel_coordinate.html) and then implement that visualization in [D3.js](https://d3js.org/) version 5.

      The prototype and D3.js versions must use the exact same encodings, but may differ slightly in the style of the axes, tick marks, titles, labels, legend placement, and so on.

The use of color to encode data is encouraged but not required by either option.

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
