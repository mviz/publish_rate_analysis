# Analyzing the publishing rate of economics PhDs

This project is analyzing the data from [The Research Productivity of New PhDs in Economics: The Surprisingly High Non-success of the Successful](https://www.aeaweb.org/articles?id=10.1257/jep.28.3.205). 

The publication rates of the students are grouped by school, and then modeled as if they are sampled from the same Poisson distribution.

The modelling was done with Monte Carlo Markov Chain sampling with PyMC3 and ArviZ, and while the model itself isn't terribly complex, the results are good.

## The Code

### Running the notebooks

The notebooks just need data, and the python libraries to be run.

Note that the visualization notebook needs the data_mapper to be run first for some of the graphs.

### The notebooks

The analysis is done in `publishing_rate_analysis.ipynb`, which covers building the Bayesian model, and validation of the simulated results.

fake_data_generator.ipynb exists to generate some fake data which could be plugged into the above analyzer, in case someone doesn't have access to the real data (which I can't include in this project due to licencing). 

data_mapper.ipynb handles some data cleanup for visualizations.


## Blog post

TODO (mviz) - link blog post.

