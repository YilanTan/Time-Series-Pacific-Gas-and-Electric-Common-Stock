# Time-Series-Pacific-Gas-and-Electric-Common-Stock
Anlysis Pacific Gas and Electric Common Stock by GARCH Model

   - Time-Series-Pacific-Gas-and-Electric-Common-Stock.Rmd: Original code of our report  
   - Time-Series-Pacific-Gas-and-Electric-Common-Stock.html: Final report    
   - PGEmonthly9621.txt: Raw data  
   
## Introduction

This report is a study on the time series analysis and model prediction of Pacific Gas and Electric common stock. During 2000 and 2001 the energy market in California experienced severe price increases which PG&E could not pass along to its customers, and the company was forced to file for bankruptcy in April 2001. In early 2019 Pacific Gas and Electric again was forced to file for bankruptcy.

## Data Sets

The data give simple monthly returns for Pacific Gas and Electric common stock for the period 1996 through 2021 and are in the file PGEmonthly9621.txt.

## Remarks

1. From our analysis, there are two bankruptcies in 2001 and 2018. The reasons are the price increase for the company to buy energy and the CA fire. The magnitude of the impact of CA fire was more dramatic, more abrupt. 
2. We use the $arima(5,0,0)(1,0,0)_{12}$ model to capture the trend and seasonal structure. 
3. The GARCH(1,1) model based on $arima(5,0,0)(1,0,0)_{12}$ captures the volatility change well (except for the significant return in Nov. 2018). The Kurtosis value, which indicates the tails of a distribution comparing to the normal one, drops from 0.6 to 3.67.
