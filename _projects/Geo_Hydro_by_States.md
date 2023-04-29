---
name: Geo and HydroPower by States
tools: [Python, HTML, vega-lite]
image: assets/pngs/geo_hydro_power_.png
description: This visualization shows Geo and HydroPower energy consumption by States
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


## How does the Generation of Clean Energy like Geothermal and Hydropower helps the residents of the USA contribute to the Green Energy Revolution

<br>

<vegachart schema-url="{{ site.baseurl }}/assets/json/Geo_Hydropower_by_States.json" style="width: 100%"></vegachart>

## Explanation of the Visualization:

The graph only shows two factors of renewable energy generation in the USA, mainly Hydropower and Geothermal energy, from a lot of different factors from the dataset like Wind Power, Gaseous Power, Solar Power and so on. The above visualization explians how many Hydropower and Geothermal energy sites are there across the USA and they are segregated in such a way that when Geopower dropdown is changed the Hydropower on the X-axis also changes. 

For example if range is provided between 35-70 in GigaWatts (gw) for Geopower than different Hydropower sites in Gigawatt Hours (gwh) will aslo be displayed and on the Y-Axis 'Count of states' can be observed where more number of Geothermal and Hydropower sites are present in each state for the following Geo and Hydro units of Power Usage.  

The graph is interactive and if as a viewer you want to understand what is going on in the visualization then it can be understood as follows. The graph basically shows the amount of energy usage/consumption done by the different states in the USA. Some states where less people live like in North Dakota or South Dakota, less energy is consumed in terms of electricity and water sources inside/below the Earth. 

More energy is used both in terms of electricity and water where more people live, like in the states of California, NY, IL and so on. The graph can help you understand in what states the most number of energy generating sites of Hydropower and Geothermal energy are and it can also help you understand how diverse and spread out the energy sites are across the United States.

*Note: For certain grouped values in the dropdown the graph will show no values, as the data had Null/no values for those grouped values in the dataset.*

## Contextual Visualization 1:

<img src='/assets/pngs/usa_energy_consumption_&_generation_types.png'>

The above visualization displays the different types of renewable energy resources that are used by the USA. The data is taken from the National Water and Energy Land Dataset (NWELD) and spatial/satellite imagery helps in determining how well these resources are bieng used. For future purposes too the above visualization helps in knowing where the expanison of renewable sites can be done. 

The most important thing is to see for Geothermal and Hydrothermal resources and how the government can build upon them. Score 1 represents that the site is not producing a good amount of energy and resources and score 3 means the site is producing a good amount of energy and resources for the nation to use.


## Contextual Visualization 2:

<img src='/assets/pngs/usa_renewable_tech_usage.png'>

This visualization shows the Energy consumption in TeraWatts by different renewable energy sites/industries, and all this was done by aerial imagery. The most amount of energy generation and usage of resources was done in the Hydropower/Hydroelectric sector and minimum generation was done by Nuclear Power sites and resources. 

This can also be understood as the Hydrogeneration is easy to produce and handle but when it comes to Nuclear power, the safety issues increase and accurate handling of all the resources takes place so that no debacle happens and everyone is safe and secure.

### References:

1. Sturtevant, J., McManamay, R. A., & Jager, H. I. (2022). U.S. national water and energy land dataset for integrated multisector dynamics research. Scientific Data, 9(1). <https://doi.org/10.1038/s41597-022-01290-w>

<div class="left">
{% include elements/button.html link="https://github.com/Shantanu97brr/Shantanu97brr.github.io/blob/main/data_proj.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

