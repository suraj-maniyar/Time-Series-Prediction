Each *.mat file contains:

[+] t - A vector of times for the measurements. The units are seconds. This is relative time from the beginning of a synchronization event on the particular datastream. This should not be used for training.
[+] y - A vector with the breathing rates in breaths per minute.
[+] x - A matrix of size N x D with the features for the corresponding measurements. N is the number of time measurements, and D is the number of features.

Each column of x corresponding to a set of features:

[+] Col 1 - Body temperature in Fahrenheit
[+] Col 2 - Heart rate in beats per minute
[+] Col 3 - Environmental temperature in Fahrenheit
[+] Col 4 - Humidity in Percentage
[+] Col 5-25 - Accelerometer features from wrist. Means from xyz (3), Variances and Covariances (6), Skewness xyz (3), Kurtosis xyz (3), Peak spectral magnitude (3) and corresponding frequency (3). 
[+] Col 26-46 - Accelerometer features from ankle. Same as above.
[+] Col 47-52 - EDA features. Mean, Linear trend (slope after linear fitting), variance, skewness, Kurtosis, and range between maximum and minimum value.
