# Masters-Thesis: A Comparative Sensitivity Analysis of Loss Functions in Machine Learning Weather Forecasting

This project contains the code and resulting plots of my Masters Thesis.

I trained a Machine Learning Weather Prediction (MLWP) model based on [GraphCast](https://arxiv.org/abs/2212.12794),
with different loss functions to analyse the impact of this choice on the results.

Model training requires downloading the [ERA5](https://www.ecmwf.int/en/forecasts/datasets/reanalysis-datasets/era5)
dataset, available from [ECMWF](https://www.ecmwf.int/). 
This was accessed as Zarr from [Weatherbench2's ERA5 data](https://weatherbench2.readthedocs.io/en/latest/data-guide.html#era5).
The evaluation was done using the [WeatherBench2](https://weatherbench2.readthedocs.io/en/latest/index.html) framework.


## overview of files and folders

*  `evaluation`: Contains the NetCDF files with the evaluated results.
*  `graphcast`: Contains a copy of the [GraphCast code](https://github.com/google-deepmind/graphcast).
the `losses.py` is edited to include the different loss functions and the `graphcast.py` file is edited to be able to select between the different loss functions.
*  `models`: Contains the parameters of the models trained with the different loss functions. These can be used to load the model and perform prediction runs.
* `plots`: Contains the plotted results.
*  `scripts`: Contains the .ipynb scripts used the download the ERA5 data, train the model, run the model, evaluate the model predictions and plot the results.
*  `weatherbench2`: Contains a copy of the [Weatherbench2 code](https://github.com/google-research/weatherbench2).
*  `requirements.txt`: Contains the necessary dependencies to run all the code.

