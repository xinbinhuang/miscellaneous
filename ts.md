

## White noise

A **time series** is **white noise** if the variables are independent and identically distributed with a mean of zero (i.e. **i.i.d with zero mean**)
- zero means
- constance variance
- no autocorrelation

#### Using ACF to diagnose white noise
- 95% of the spikes in the ACF would lie within **±2 / √T**, where *T* is the length of he time series.


## Stationarity

- no trend & no seasonality
- may have cyclic behaviors with no predictable patterns in the long term.
  - roughly horizontal with constance variance.



## STL

> Seasonal and Trend decomposition using LOESS

After decomposition, we have:

- trend-cyclic
- Seasonal component
- remainder

To get the Seasonal-adjusted series: 1) subtract the original series by the seasonal component, a.k.a the sum of trend-cycle and remainder


### Reference

- [Is it unusual for the MEAN to outperform ARIMA?](https://stats.stackexchange.com/questions/124955/is-it-unusual-for-the-mean-to-outperform-arima/125016#125016)
- [Is STL a good technique for forecasting than ARIMA](https://stats.stackexchange.com/questions/298560/is-stl-a-good-technique-for-forecasting-instead-of-arima)
- [Forecast: STL+ARIMA vs ARIMA](https://stackoverflow.com/questions/29347791/r-forecast-season-and-trend-of-data-using-stl-and-arima)
