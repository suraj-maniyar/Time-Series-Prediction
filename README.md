# Respiratory-Rate-Estimation

## Project description
This project aims to predict the respiratory rate of an individual which is a time-series data with temporal dependence. 

## Data
The data provided is the accelerometer data worn by the individual on the wrist and the ankle. An EDA is performed on this data and 52 features are provided as the input. 

A sample part of the respiratory curve is shown below:

<img src="assets/RR_zoomed.png" width="60%">

The entire respiratory rate available from the data is spread across time as shown:

<img src="assets/RR_zoomed.png" width="60%">


## Approach

### Data Pre-processing

We observe that there are spikes occurring in the dataset due to noisy measurements. So to remove the noise, we take the first order derivative and set a threshold 

