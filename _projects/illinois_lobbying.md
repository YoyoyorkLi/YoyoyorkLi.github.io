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
By Jaylin Chen and York Li
<br><br>

Taxpayer-funded lobbying in Illinois is on the rise, and it is important to keep track of the trends and patterns! This interactive chart highlights the top five business entities in a selected city in the state of Illinois and year, ranked by the number of unique clients they served. Clicking on an entity reveals a second chart that displays how its client count has changed across years.

For this plot, Two datasets from the illinois governmental data website were used. The first dataset entails all lobbying entities in the state of Illinois, the second dataset includes information about their clients. Both datasets weren joined by
the client key to create a master dataset. After extensieve data cleaning, such as eliminating extra and renaming certain columns,
We ended up with a dataset of companies, entities that lobby for them, and the amount of lobbists they have.
<br><br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/illinois_clients.json" style="width: 100%"></vegachart>

<br>

For context, the 15 companies with the most amount of lobbiests and the 15 lobbying entities with the most amount of clients are also plotted. 
<vegachart schema-url="{{ site.baseurl }}/assets/json/client_info.json" style="width: 100%"></vegachart>

<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/ent_info.json" style="width: 100%"></vegachart>

# Next Steps
<br>
Additional analysis could be conducted if more data becomes available. For instance, the company's lobbying impact could be examined in greater depth by incorporating variables such as total lobbying expenditure, number of bills influenced, policy focus areas, and year-over-year trends. Visualizations could compare spending against client outreach frequency, highlight the most active lobbying periods, and track changes in engagement over time. Furthermore, integrating datasets on legislation outcomes or industry sectors would allow for more robust insights into effectiveness and influence. With richer data, predictive modeling could also be applied to estimate lobbying success or forecast future activity.
<br><br><br><br>

<div class="left">
{% include elements/button.html link="https://data.illinois.gov/browse?sortBy=last_modified&pageSize=20&category=Government+and+Public+Employees&page=1" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/YoyoyorkLi/YoyoyorkLi.github.io/blob/main/python_notebooks/illinois_lobbying.ipynb" text="The Analysis" %}
</div>
