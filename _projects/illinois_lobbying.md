---
name: Interactive Lobbying Entities in Illinois
tools: [Python, HTML, Bqplot]
image: assets/pngs/lobby.png
description: Lobbying Entities in the State of Illinois and Their Clients!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Interactive Lobbying Entities in Illinois
<br>

Taxpayer-funded lobbying in Illinois is on the rise, and it is important to keep track of the trends and patterns! This interactive chart highlights the top five business entities in a selected city in the state of Illinois and year, ranked by the number of unique clients they served. Clicking on an entity reveals a second chart that displays how its client count has changed across years.


<vegachart schema-url="{{ site.baseurl }}/assets/json/illinois_clients.json" style="width: 100%"></vegachart>

<br><br>


<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/YoyoyorkLi/YoyoyorkLi.github.io/blob/main/python_notebooks/bigfoot.ipynb" text="The Analysis" %}
</div>