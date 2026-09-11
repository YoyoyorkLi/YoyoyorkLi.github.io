---
name: Turning My Fitbit Air Into WHOOP
tools: [PostgreSQL, Data Visualization]
description: Upgrading my Google Fitbit Air Into WHOOP with custom metrics and a Postgres Backend.
image: assets/pngs/whoop.png
---
### Overview
---
My Fitbit's Google Health app only shows raw numbers, so I built my own web app, with a strain score, a recovery score, and a sleep score, computed nightly and stored in a Postgres backend behind an installable PWA modeled on WHOOP's own Day / Workouts / Drinks / Trends layout.

My app also tracks how alcohol shows up in next-morning HRV and recovery.

### Live Demo
*(Synthetic data — sign-in is disabled for this demo.)*

<div style="width: 100%; overflow: auto; -webkit-overflow-scrolling: touch;">
  <iframe
    src="{{ site.baseurl }}/assets/html/preview.html?demo=1"
    style="width: 100%; min-width: 100%; height: 1400px; min-height: 1400px; border: none; display: block;"
    title="Pulse — Recovery Dashboard">
  </iframe>
</div>
