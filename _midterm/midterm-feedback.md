---
title: Midterm Feedback
navbar: Guides
layout: guides
key: 1.3

tags:
- text: 'Updated'
  type: 'is-primary'

assignments:
  - text: 'Midterm Beta Release'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908101'

  - text: 'Midterm Prototype Demonstration'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908141'

  - text: 'Midterm Prototype Feedback'
    link: 'https://usfca.instructure.com/courses/1590235/assignments/6908142'

  - text: 'Midterm Feedback Form'
    info: '(Google Form)'
    link: 'https://docs.google.com/forms/d/e/1FAIpQLSeHDbp9F4aeicWeu-MkQwb830Bar57qcLDQNO-aZne5HWI7aQ/viewform?usp=sf_link'

blurb: |
  <p>Instead of a midterm exam, all students must complete a midterm group project. This guide describes the midterm prototype feedback process.</p>
---

{% assign midterm = site.data.midterm %}

<i class="fas fa-exclamation-triangle"></i>
Attendance is mandatory for these in-person participation exercises. There will be no live-stream on these days.
{: .notification .is-danger}

## Overview

Getting both objective and subjective evaluation is critical to designing effective visualizations. This two day in-person participation exercise will allow groups to get this type of feedback from multiple different peers. Groups will switch off between presenting their projects and providing peer feedback for other projects.

<table class="table is-hoverable is-auto">
<thead>
  <tr>
    <th>Group</th>
    <th>Team Members</th>
    <th>Prototype Presentation Date</th>
    <th>Prototype Feedback Date</th>
  </tr>
</thead>
<tbody>
{% assign sorted_groups = midterm.groups | sort: "link" %}
{%- for group in sorted_groups %}
<tr>
  <td>{{ group.link }}</td>
  <td>{{ group.team | join: ", " }}</td>
  <td>{{ group.proto |date: "%A %B %d, %Y" }}</td>
  <td>
    {%- if group.proto == site.data.midterm.feedback.tue %}
      {{ site.data.midterm.feedback.thu |date: "%A %B %d, %Y" }}
    {% else %}
      {{ site.data.midterm.feedback.tue |date: "%A %B %d, %Y" }}
    {% endif -%}
  </td>
</tr>
{% endfor -%}
</tbody>
</table>

## Presentation

Each group must lead **25 minute** presentation and discussion of their project **three times** for different feedback groups throughout the class, with 10 minute breaks between each presentation. The presentation schedule is as follows:

| Tuesday 3/03   | Thursday 3/05  |
|:---------------|:---------------|
| {{ midterm.chinchillas.link }} | {{ midterm.datalization.link }} |
| {{ midterm.persimmon.link }}   | {{ midterm.visualizers.link }} |
| {{ midterm.enigma.link }}      | {{ midterm.datasetgo.link }} |
| {{ midterm.windows10.link }}   | {{ midterm.colorisfake.link }} |
| {{ midterm.dataviz.link }}     | {{ midterm.datadmin.link }} |
{: .table .is-hoverable .is-auto }

During the presentation, groups should start with a brief overview of the project theme. Make sure the feedback group is able to properly load the project website. Then, for each visualization, explain the following:

  1. **What** subset of data is being visualized
  2. **Why** you created that visualization
  3. **How** that visualization is encoded
  4. **How** it fits into the overall theme

Finally, answer questions and ask for feedback on that specific visualization. Make sure to leave between 5-10 minutes for the feedback group to enter written comments on Canvas!

Presentation groups are encouraged to switch off who is presenting and who is taking notes. These roles can switch per visualization within each session, or one person can present for an entire session and then switch to taking notes. (This will also be great practice for the midterm project presentation later.) **All group members must participate in the presentation in some way.**

#### Layout

The room layout for **presenting** groups is shown below. If your group is presenting, find your location and setup. You will be in that location for the entire time. If your group is providing feedback, you will need to move to the location of the presenting group you are assigned for each of the three sessions.

<figure class="image">
<img src="/images/midterm-layout.svg" style="width: 700px; max-width: 100%;"><br/>
<caption>Room layout for presenting groups.</caption>
</figure>

Everyone just needs to be close enough to hear each other, but does not need to be able to view the same laptop screen at once. Instead, everyone should use the peer review feature in Canvas to directly access the visualizations being discussed on their own laptop screens.

## Feedback

[<i class="fas fa-edit"></i> Feedback Form](https://docs.google.com/forms/d/e/1FAIpQLSeHDbp9F4aeicWeu-MkQwb830Bar57qcLDQNO-aZne5HWI7aQ/viewform?usp=sf_link)
{: .button .is-primary .inherit }

Each group must provide feedback for **three groups** on the day they are not presenting. The  **Tuesday** feedback schedule is as follows:

|                | Session 1     | Session 2       | Session 3       |
| Feedback Group | 4:45p – 5:10p | 5:20pm – 5:45pm | 5:55pm – 5:20pm |
|:---------------|:--------------|:----------------|:----------------|
| {{ midterm.datalization.link }} | {{ midterm.chinchillas.form }} {{ midterm.chinchillas.link }} | {{ midterm.persimmon.form }}  {{ midterm.persimmon.link }}   | {{ midterm.enigma.form }}      {{ midterm.enigma.link }}      |
| {{ midterm.visualizers.link }}  | {{ midterm.persimmon.form }}   {{ midterm.persimmon.link }}   | {{ midterm.enigma.form }}     {{ midterm.enigma.link }}      | {{ midterm.windows10.form }}   {{ midterm.windows10.link }}   |
| {{ midterm.datasetgo.link }}    | {{ midterm.enigma.form }}      {{ midterm.enigma.link }}      | {{ midterm.windows10.form }}  {{ midterm.windows10.link }}   | {{ midterm.dataviz.form }}     {{ midterm.dataviz.link }}     |
| {{ midterm.colorisfake.link }}  | {{ midterm.windows10.form }}   {{ midterm.windows10.link }}   | {{ midterm.dataviz.form }}    {{ midterm.dataviz.link }}     | {{ midterm.chinchillas.form }} {{ midterm.chinchillas.link }} |
| {{ midterm.datadmin.link }}     | {{ midterm.dataviz.form }}     {{ midterm.dataviz.link }}     | {{ midterm.chinchillas.form }}{{ midterm.chinchillas.link }} | {{ midterm.persimmon.form }}   {{ midterm.persimmon.link }}   |
{: .table .is-hoverable .is-auto }

For example, in session 1, the {{ midterm.datalization.link }} group will be give feedback for the {{ midterm.chinchillas.link }} group. Then, the {{ midterm.datalization.link }} group will move and give feedback for the {{ midterm.persimmon.link }} group in session 2 starting at 5:20pm. Finally, {{ midterm.datalization.link }} group will be give feedback to the {{ midterm.enigma.link }} group during the last session at 5:55pm. Then, Thursday, the {{ midterm.datalization.link }} will present their project and get feedback from other groups.

The **Thursday** feedback schedule is as follows:

|                | Session 1     | Session 2       | Session 3       |
| Feedback Group | 4:45p – 5:10p | 5:20pm – 5:45pm | 5:55pm – 5:20pm |
|:---------------|:--------------|:----------------|:----------------|
| {{ midterm.chinchillas.link }} | {{ midterm.visualizers.form }}  {{ midterm.visualizers.link }}  | {{ midterm.datasetgo.form }}    {{ midterm.datasetgo.link }}    | {{ midterm.colorisfake.form }}  {{ midterm.colorisfake.link }}  |
| {{ midterm.persimmon.link }}   | {{ midterm.datasetgo.form }}    {{ midterm.datasetgo.link }}    | {{ midterm.colorisfake.form }}  {{ midterm.colorisfake.link }}  | {{ midterm.datadmin.form }}     {{ midterm.datadmin.link }}     |
| {{ midterm.enigma.link }}      | {{ midterm.colorisfake.form }}  {{ midterm.colorisfake.link }}  | {{ midterm.datadmin.form }}     {{ midterm.datadmin.link }}     | {{ midterm.datalization.form }} {{ midterm.datalization.link }} |
| {{ midterm.windows10.link }}   | {{ midterm.datadmin.form }}     {{ midterm.datadmin.link }}     | {{ midterm.datalization.form }} {{ midterm.datalization.link }} | {{ midterm.visualizers.form }}  {{ midterm.visualizers.link }}  |
| {{ midterm.dataviz.link }}     | {{ midterm.datalization.form }} {{ midterm.datalization.link }} | {{ midterm.visualizers.form }}  {{ midterm.visualizers.link }}  | {{ midterm.datasetgo.form }}    {{ midterm.datasetgo.link }}    |
{: .table .is-hoverable .is-auto }

During each feedback session, feedback groups must:

  1. Find the assigned presentation group. Look at the schedule above to see which group you are assigned, and at the layout below for where this group will be located.
  2. Load the presentation group project website on your laptop. The website is linked in the schedule above.
  3. Load the peer feedback rubric for the presentation group. Canvas cannot support group peer review, so enter your feedback in the [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSeHDbp9F4aeicWeu-MkQwb830Bar57qcLDQNO-aZne5HWI7aQ/viewform?usp=sf_link) instead. The <i class="fas fa-user-edit"></i> icon in the schedule will auto-fill the group name for you.
  4. During the presentation, ask clarification questions and give verbal feedback.
  5. After the presentation, leave written feedback on Canvas. You will need 5-10 minutes for this process.

All feedback must be professional, substantive, constructive, and students must follow the [Student Conduct Code](https://usf-cs360-spring2019.github.io/syllabus.html#behavioral-expectations) of the university. Students are encouraged include the following in their feedback:

  - Feedback of the visualizations using **objective evaluation** concepts discussed in class (e.g. lie factor, data density, data/ink ratio).

  - Feedback of the visualizations using **subjective evaluation** (sensitively and constructively delivered) regarding the design.

  - Feedback of the visualizations regarding the **relevance to theme**, stated goals, and website cohesiveness.

  - Discussion of technical details where appropriate (e.g. suggestions on different approaches in D3, prototype tools, data preprocessing steps).

Students are encouraged to provide verbal feedback during the presentation, but *must* provide detailed written feedback to get credit for the feedback exercise.

Once a feedback session is over, there will be a 10 minutes break. During that break, you must finish writing up your feedback on Canvas and find the presenting group for the next session.
