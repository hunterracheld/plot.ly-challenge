To view this dashboard: Belly_Button_Biodiversity > index.html
NOTE: This dashboard must be viewed on a local server to avoid CORS errors.

The [Belly Button Biodiversity dataset](http://robdunnlab.com/projects/belly-button-biodiversity/) catalogs the microbes that colonize human navels.

The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.

## app.js

1. Uses the D3 library to read in `samples.json`.

2. Creates a horizontal bar chart with a dropdown menu to display the top 10 OTUs found in that individual.

* Uses `sample_values` as the values for the bar chart.

* Uses `otu_ids` as the labels for the bar chart.

* Uses `otu_labels` as the hovertext for the chart.

3. Creates a bubble chart that displays each sample.

* Uses `otu_ids` for the x values.

* Uses `sample_values` for the y values.

* Uses `sample_values` for the marker size.

* Uses `otu_ids` for the marker colors.

* Uses `otu_labels` for the text values.

4. Adapts the Gauge Chart from <https://plot.ly/javascript/gauge-charts/> to plot the weekly washing frequency of the individual.

5. Displays the sample metadata, i.e., an individual's demographic information.

6. Displays each key-value pair from the metadata JSON object on the page.

7. Updates all of the plots any time that a new sample is selected.


### About the Data

Hulcr, J. et al.(2012) _A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable_. Retrieved from: [http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)



