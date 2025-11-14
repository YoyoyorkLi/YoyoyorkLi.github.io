---
name: Interactive Bigfoot Sighting Plot
tools: [Python, HTML, JavaScript]
image: assets/pngs/bigfoot.png
description: Bigfoot sightings in the U.S filtered by state, visibility and more!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Interactive Bigfoot Sighting Plot
<br>

[Bigfoot](https://en.wikipedia.org/wiki/Bigfoot) is a large mythical creature said to inhabit forests in North America. For this project, Bigfoot sighting data was filtered then plotted by season and state, highlighting average visibility and temperature to reveal potential trends.

### Plot seperated by season

<vegachart schema-url="{{ site.baseurl }}/assets/json/bigfoot_chart1.json" style="width: 100%"></vegachart>

<br>
By seperating the data by season, the visualization highlights how environmental conditions and sighting patterns shift throughout the year.
<br><br>

### Plot with state sightings
<br>
<vegachart schema-url="{{ site.baseurl }}/assets/json/bigfoot_chart2.json" style="width: 100%"></vegachart>
<br>
Sightings are also plotted by state, making it easy to compare regional differences.

<br>


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/YoyoyorkLi/YoyoyorkLi.github.io/blob/main/python_notebooks/bigfoot.ipynb" text="The Analysis" %}
</div>