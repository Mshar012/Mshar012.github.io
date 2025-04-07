---
name: Homework 5
tools: [Python,Altair, Vega-Lite]
image: /assets/pngs/hwimage.png
description: A Bar chart showing number of buildings managed by each Illinois state agency and a histogram displaying the number of buildings by city, filtered by agency.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Plot 1: Number of Buildings by agency 

<vegachart schema-url="{{ site.baseurl }}/assets/plot/bar.json" style="width: 100%; height: 500px;"></vegachart>

This bar chart reflects the number of buildings managed by each Illinois state agency. I used Altair to encode the agency names on the x-axis and the number of buildings on the y-axis, sorting the values in descending order to enhance readability. By examining the chart, we can easily identify which agencies manage the most buildings; for example, the Department of Natural Resources has the highest count. The agency names are encoded as nominal data, while the y-axis uses a quantitative count aggregation. The only data transformation I applied was the default grouping performed by Altair’s count() function.

---

# Plot 2: Distribution of Buildings Across Cities by Agency 

<vegachart schema-url="{{ site.baseurl }}/assets/plot/hist.json" style="width: 100%; height: 500px;"></vegachart>

Write up for the 2nd Plot:

This interactive histogram displays the number of buildings by city, filtered by agency. It allows users to easily identify where a specific agency has the highest number of buildings. The x-axis represents city names (nominal), while the y-axis shows the count of buildings (quantitative). To add interactivity, I included a dropdown menu that enables users to select an agency and instantly view how its buildings are distributed across different cities.

---

## Dataset and Python Notebook Links

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/Mshar012/Mshar012.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis Notebook" %}
</div>


