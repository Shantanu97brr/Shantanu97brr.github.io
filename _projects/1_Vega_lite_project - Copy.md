---
name: IS 445 Assignment10
tools: [Python, altair, vega-lite]
image: assets/pngs/usa_states.png
description: Analyzing data related to reported sightings of Bigfoot or other similar cryptids in various locations across the United States of America.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Visualization 1 - Number of Sightings Binned by High Temparatures per State

I displayed a heatmap to compare and see what insights can be gained when the temperature is high in the given states and what happens when the frequency is high and low respectively. 

Again the highest frequency of sighting and more information was in the state of Washington but surprisingly the average frequency states were California and Ohio in the 200 range and the lowest were in states like Nevada and North Dakota. If I had more time I would have tried to do explore different binning options, more color schemes and most importantly I would have tried it for different Counties but there we so many counties that it was a bit had to display the information correctly on the X-Axis, maybe I would have tried to flip the axis in a vertical manner. 

The visualization highlights the feature that the higher the temperature the more incidents might have happened which kind of shows a correlation between the high_temp and states columns around the year. If I had more time I would have tried to add a count of frequency too in the visualization above.

Especially here I used the altair syntax where I kept all the displaying code inside the Chart.dictionary() function/method. I also used .add-selection() function with a brush so that I am able to select the given heatmaps and those selected bars will also change later in the interactive visualization.

The same vega-lite code was chosen from HW9. The specifications/coding and modifications had to be added inside
```
alt.Chart.from_dict()
```
and comments had to be replaced from '//' to '#'.

<vegachart schema-url="{{ site.baseurl }}/assets/json/state_heat_map.json" style="width: 100%"></vegachart>


# Visualization 2: Frequency of Sightings per State

The plot below includes a histogram plot of the Bigfoot sightings/other cyrptic incidents that happened during the course of year, I have used features/columns that I have used for my analysis county, state, high temperatures and what is caused by all the features in the country of USA. I used the height and width by using the javascript coding and set it to 500 as it displayed the plots accurately and in as way that they can be understood easily. 

The Frequency is used on the Y-Axis to see how many times the sighting/incidents happened, the scale goes from 0 - 600, and the X-axis has all the state information on them. The highest one is of Washington state and the states like Nevada, Delaware, and North Dakota. 

If I had more time I would have seen if these bar charts show some statistical ability like if they are left skewed or right skewed and what more information can be understood as we glance or observe onto the bar/histogram chart. I could have also dwelled in the number of bins and changed it to see what analysis can be done and I would have also tried to play with the color schemes a bit too.

Some other/different altair syntax where I kept all the displaying code inside the Chart.dictionary() function/method. This slight change in the code helped me to display my visualization in a manner of vega-lite, altair, javascript, and deployment on Github.

The same vega-lite code was chosen from HW9. The specifications/coding and modifications had to be added inside
```
alt.Chart.from_dict()
```
and comments had to be replaced from '//' to '#'.

<vegachart schema-url="{{ site.baseurl }}/assets/json/state_hist.json" style="width: 100%"></vegachart>

# Visualization 3 - Dashboarding & Interactivity

For interactive dashboard purposes also I again used the altair syntax where I kept all the displaying code inside the Chart.dictionary() function/method and this time I used another function called '.transform_filter() with a brush to maintain/display the visualization side by side. Other stuff like height and width were used accordingly to keep the visalization accurately visible.

<vegachart schema-url="{{ site.baseurl }}/assets/json/dashboarding.json" style="width: 100%"></vegachart>

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

