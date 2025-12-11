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




# Contextual Visualizations



<vegachart schema-url="{{ site.baseurl }}/assets/json/weeds.json" style="width: 100%"></vegachart>

<vegachart schema-url="{{ site.baseurl }}/assets/json/waste.json" style="width: 100%"></vegachart>

# Information
For my first visualization, it is an interactive graph where the user can select a month and a year and the graph will show all the different types of complaints that were filed and how many for each. The purpose of this is to visualize which complaints were more popular and less popular for a given specific month and year. For example, during the summer months, you can notice a trend that weeds/grass always tends to have the most complaints no matter the year. 

For both these contextual visualizations, I'm showing the distribution in the fees paid for each case. The first visualization is specifically for fees paid for Weeds/Grass complaints and the second visualization is for Municipal Waste complaints. If you look closely, you'll notice that the typical fees paid for municipal waste are slightly higher than the fees paid for weeds/grass. 

<!-- these are written in a combo of html and liquid --> 

<div class="center">
{% include elements/button.html link="https://github.com/WorstProgrammer7636/worstprogrammer7636.github.io/blob/main/python_notebooks/finalproject.ipynb" text="Python Notebook" %}
</div>

