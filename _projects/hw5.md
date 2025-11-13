---
name: HW5 Visualizations
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: HW5 Visualizations
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# First Viz

For this first visualization, I'm mapping out all the buildings spread out across all the years (which are non zero) based on their median square footage. I based the y axis on symlog instead of linear because there are a few buildings with square footage that is extremely high that stretches out the distribution of values too much to make it readable. For my coloring, I decided to give different colors to each point depending on what that building was used for. For example, an assembly building is a certain color while business is another. This makes it easy to distinguish the many different types of buildings. Going back to me not using any zero values, let me elaborate. There were a lot of values that were zero for the "year" column. This seemed weird to me and it also stretched the graph a lot so i just decided to remove them by filtering them out of the dataframe. For the interactivity, i made it so you can choose a specific usage description (building type) to highlight the points of. For example, if you want to see only the health care buildings more easily, you can select that and it'll highlight all of the healthcare building points. 

<vegachart schema-url="{{ site.baseurl }}/assets/json/years.json" style="width: 100%"></vegachart>




# Second Viz

For the second visualization, I simply got the frequency of the top cities and created a bar chart to visualize the most popular cities for the buildings. For the coloring, I just let altair automatically select different colors for the different bars to make it easy for the reader to see the difference in frequencies between the top cities. In order for me to make this visualization work, I had to do .head(10) to pick out the top 10 cities and then reset index so altair can properly read the data. For this visualization, there isn't any interactivity and is a more straightforward visualization.

<vegachart schema-url="{{ site.baseurl }}/assets/json/cities.json" style="width: 100%"></vegachart>



<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/WorstProgrammer7636/worstprogrammer7636.github.io/blob/main/python_notebooks/is445visualizations.ipynb" text="The Analysis" %}
</div>

