# Retail-Forecasting-Project

## Objective: To forecast a real time series using ETS and ARIMA models.

## Data: Each student will be use a different time series, selected using their student ID number.
set.seed(12345678)
myseries <- aus_retail |>
  filter(!(`Series ID` %in% c("A3349561R","A3349883F","A3349499L","A3349902A",
                        "A3349588R","A3349763L","A3349372C","A3349450X",
                        "A3349679W","A3349378T","A3349767W","A3349451A"))) |>
  filter(`Series ID` == sample(`Series ID`,1))
  
## Report:
Should produce forecasts of the series using ETS and ARIMA models. Write a report in Rmarkdown format of the analysis explaining carefully what have done and why have done it.
