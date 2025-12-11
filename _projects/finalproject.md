---
name: Final Project Visuzliations
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Final Project Visualizations
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Final Project
<h2>Group Members: Max Tao</h2>
<a href='https://data.illinois.gov/Local-Government/City-Of-Urbana-Nuisance-Complaints/64q4-57u5/about_data'>Link to Dataset</a>

# First Viz

Complaints
<vegachart schema-url="{{ site.baseurl }}/assets/json/complaints.json" style="width: 100%"></vegachart>




# Second Viz

For the second visualization, I simply got the frequency of the top cities and created a bar chart to visualize the most popular cities for the buildings. For the coloring, I just let altair automatically select different colors for the different bars to make it easy for the reader to see the difference in frequencies between the top cities. In order for me to make this visualization work, I had to do .head(10) to pick out the top 10 cities and then reset index so altair can properly read the data. For this visualization, there isn't any interactivity and is a more straightforward visualization.

<vegachart schema-url="{{ site.baseurl }}/assets/json/weeds.json" style="width: 100%"></vegachart>

# Third Viz

<vegachart schema-url="{{ site.baseurl }}/assets/json/waste.json" style="width: 100%"></vegachart>



<!-- these are written in a combo of html and liquid --> 

<div class="center">
{% include elements/button.html link="https://github.com/WorstProgrammer7636/worstprogrammer7636.github.io/blob/main/python_notebooks/finalproject.ipynb" text="Python Notebook" %}
</div>

