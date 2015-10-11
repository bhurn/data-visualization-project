# data-visualization-project
Udacity Data Analyst Project 5

Summary
This explanatory visualization shows the changes in the Bureau of Labor Statistics Employment-Population Ratios for men and for women over the time period from 1948 Q1 through 2015 Q3. The Employment-Population Ratio is the ratio of the number of people employed to the population of people ages 16 and up. The line chart indicates two distinct trends: the share of women particpating in the workforce grew from the 1940s through the 1980s, and the proportion of men working has been consistently declining. The participation gap between men and women has declined from 53 percentage points in 1948 to 11 points in the latest quarter reported.

Design
Because the data represents two distinct time series, a line chart was a natural choice for this project. The initial version was surprisingly simple to create using dimple and the skeleton code from the course. This version included left-justification for the header and footer (to avoid misalignment between centered headers and the chart in wide browser windows), axis titles, values as numbers (rather than percents), and the default dimple draw animation. Multiple reviewers commented that the default colors and legend formatting (Men above Women, which mimics the order of the lines in the chart) helped make it immediately clear which line represented which series, so that formatting was retained for the final version.

Based on some confusion from reviwers about meaning of the metric, I added a more explanatory subtitle, including the age ranges (16+) included in the data. Because the point of the chart wasn't entirely clear, I added a more descriptive title as well. The additional annotations and animations (creating an author-driven narrative) helped highlight key insights that the reviewers had missed.

I updated the code to convert the y-axis values to decimals (from the original values based on a scale from 0 to 100) and to include percentage-formatted axis labels to make it clear that the values were in fact percentages. Reviewers then understood that the axes represented percentages and years, so both axis tiles were deleted to reduce chart junk. I also faded out the box representing the 2008 recession based on feedback that it made the final note difficult to read.

Feedback
Three people reviewed the visualization over the course of its development. Their feedback is summarized below.
  - The line chart is clearly an indication of trends over years
  - The initial animation was a nice touch.
  - If you hover on the lines you get point by point information again in an animated fashion.
  - The chart indicates the source of the data and includes a clear key.
  - The axis contents are clearly percentages and dates.
  - What ages define men and women?
  - My first thought is that the numbers should equal 100 but I am looking further into whether that is actually true.
  - Not clear what "Employment-Population Ratio" means.
  - Woman have clearly grown in the workforce and are now paralleling men. Men have dropped slightly.
  - The ratio of women who have entered the workforce since 1948 is substantial.
  - The animations highlight the trend for women and men in a parllel fashion.
  - The 2008 recession disparate impact insight was not something that was initially seen without the animation.
  - The rectangle for the recession made it harder to read the final note.

Resources
The following resources were used in this project:
  - Udacity class source code
  - dimple documentation and examples at dimplejs.org
  - d3.js documentation and examples at d3js.org
  - SVG Basic Shapes and D3.js at https://www.dashingd3js.com/svg-basic-shapes-and-d3js
  - javascript help files at developer.mozilla.org
  - javascript and d3 forum discussions at stackoverflow
  - javascript, CSS, and HTML help files at w3schools.com
