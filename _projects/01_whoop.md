---
name: Turning My Fitbit Air Into WHOOP
tools: [PostgreSQL, Data Pipeline]
description: Upgrading my Google Fitbit Air Into WHOOP with custom metrics and a Postgres Backend.
image: assets/pngs/whoop.png
---
### Overview
---
My Fitbit's Google Health app only shows raw numbers with medicore UI, so I built my own web app.

The app provides a clear strain, recovery, and a sleep score, computed nightly and stored in a Postgres backend. The installable PWA shows Day / Workouts / Drinks / Trends layout.

The app also tracks how alcohol affects next-morning sleep and recovery. See GitHub repo [here](https://github.com/YoyoyorkLi/fitbitair-pwa).

### Demo
*(Synthetic data — sign-in is disabled for this demo.)*

<div style="width: 100%; overflow: auto; -webkit-overflow-scrolling: touch;">
  <iframe
    src="{{ site.baseurl }}/assets/html/preview.html?demo=1"
    style="width: 100%; min-width: 100%; height: 1400px; min-height: 1400px; border: none; display: block;"
    title="Pulse — Recovery Dashboard">
  </iframe>
</div>
