# Simple models for COVID-19 hospitalizations

The models built here use the HHS Protect daily COVID-19 hospital admissions data.

We create a set of simple baseline models that project existing trends into the future. Each baseline has a different set of options specified. We then combine the baseline models into a single ensemble forecast.


## setup 

1. Install the [simplets](https://github.com/reichlab/simplets) R package ("simple time-series" models).
2. Install the epitools R package (as of Jan 6, 2022, you need to install [a specific branch on a specific fork](https://github.com/elray1/epitools/tree/outlier_correction)).
3. Install the [hubEnsembles](https://github.com/reichlab/hubEnsembles) R package.
4. Install the [covidHubUtils](https://github.com/reichlab/covidHubUtils) R package.

## workflow

1. run `make all` in root directory
2. submit forecast submission file from `weekly-submission/forecasts/UMass-trends_ensemble/` to the COVID-19 Forecast Hub as a PR.
3. commit and push generated CSV files from all models and the PDF of plots from JUST the trends_ensemble model. 
