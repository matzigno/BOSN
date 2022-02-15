For each image file, we store the x and y values of every line in the plot.
All data is stored in json files.

time series and ACF values are stored in steem_timeseries.json and sbd_timeseries.json for STEEM and SBD analysis respectively.

While data for the study of KDE and CDF is stored in aggregated.json

Note: for figures we use smoothing 

e.g: 

from scipy.ndimage.filters import uniform_filter1d

y = uniform_filter1d(y, size = running_avg_window)

with running_avg_window = 7