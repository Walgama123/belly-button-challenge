
<h1 align="center">Belly Button Biodiversity Dashboard</h1>

## Background.
Build an interactive dashboard to explore the Belly Button Biodiversity.  which catalogs the microbes that colonize human navels.
The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.

## Data sources.
- [Belly Button Biodiversity](https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json)

## Tools and libraries used
- [D3.js](https://d3js.org/d3.v7.min.js)
- [plotly/plotly.js](https://cdn.plot.ly/plotly-latest.min.js)
- [bootstrap](https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css)

## Activities. 
- Import data from website using d3.json.
- Analyzed object and extract different data available.  
  - Names - Sample ID list.
  - Metadata - Demographic information of the samples.
  - otu_ids -  ID of the bacteria.
  - otu_labels - Name of the bacteria.
  - sample_values - Value of the bacteria found in the sample.
  
- Change the HTML values of the index.html file using D3
- Create functions for refresh the data and plot the graphs. 

## functions.
- init() - Function automatically called at the time of page refresh and deploy the data of first record by  calling other functions.
- buildMetadata(parameter_name) - This function accept one parameter (sample ID) filter the meta data for a given sample ID. 
- buildCharts(parameter_name) - This function accept one parameter (sample ID) and filter bacteria names and values and plot the graphs. 


## Graphs.
- [Bubble chart- Distribution of the values of each bacteria for a given sample ID](images/bacteriacultures.png)  
- [Horizontal bar chart- Plot the top 10 bacteria values for a given sample ID](images/top10Bacteria.png)


## Folders and files.
- Root folder
  - [index.html](index.html)
  - [samples.json](samples.json)
  - [README.md](README.md)
- static/js
  - [app.js](static/js/app.js)
- Images
  - [Bubble chart](Images/bacteriacultures.png)  
  - [Horizontal bar chart](Images/top10Bacteria.png)
