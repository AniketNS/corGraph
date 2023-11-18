# correlation-matrix-as-network
I recently found [gpt-pilot](https://github.com/Pythagora-io/gpt-pilot) and wanted a semi-complex project to give it a try with. I decided to port an app in development for [MicrobiomeDB](microbiomedb.org) to an R Shiny app.

## Someday, hopefully, this will be:
An R Shiny app to visualize a correlation matrix as a network. For the first implementation I'm anticipating trying to produce a bipartite network for displaying correlation matrices produced w two disparate data.frames.
A practical example, from the microbiome space, might be the correlations between various taxonomic abundance and pathway abundance. In this example, taxa would represent a column of nodes in the visualization and pathways a second,
and separate column of nodes. Links between these two columns of nodes are weighted by the absolute value of the correlation coefficient and colored by the direction of the correlation.

## Currently, this is:
An R Shiny app that uploads a file and attempts to validate it.
Run what I currently have, from R, like this: `shiny::runApp(launch.browser=T)`