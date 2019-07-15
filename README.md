# Stock-Price-Forecasting

Using Autoregressive Integrated Moving Average (ARIMA), 
this projects forecasts future stock prices based on the past data alone. 

## Getting Started
First train the model using training command given below or see the already trained stocks.After that,
using visualization.py we can predict the future prices.
### Dependencies
```
pip install -r requirements.txt
```
#### Training 
To find the optimal values model run:
```
python train_agent.py --choice [ENTER A STOCK HERE]
```
To display a list of the available stocks run:
```
python train_agent.py --list show
```
#### Visualize 
To visualize the data run:
```
python visualize_main.py --choice [ENTER STOCK HERE] --data_display [simple
 OR forecast]
```
###### --data_display simple
This visualizes the past stock price history, without the forecasted price

###### --data_display forecast
This displays the past data along with the forecasted price history of the stock.

## Conclusion
 Our model predicted the future prices for stocks in a very general sense,strongly. We believe this is not because of the model itself, but because of 
 the market performance during and after the provided data. 
 Our model was mostly unsuccessful in ignoring the noise, even with our best efforts to stationarize the data.
 
#### What could be improved As previously stated in our conclusion, the data we provided allows theagent to learn a false hypothesis about the market. 
To improve this one could collect more data that encompasses a severe market correction.

