This is the reproduce of the paper https://link.springer.com/article/10.1007/s42979-022-01019-x

1.To reproduce the result, just open COVID_ARIMS_LSTM.ipynb 
# Metrics
res_lstm_ConfirmedCases, mse, rmse, msle, rmsle, mae, mape = evaluate_lstm(forcast_ConfirmedCases,train_rate,lstm_size)
print('>>>', forcast_ConfirmedCases.columns.values[0], 'LSTM Results MSE = %.5f RMSE = %.5f MSLE = %.5f RMSLE = %.5f MAE = %.5f MAPE = %.5f' % (mse, rmse, msle, rmsle, mae, mape))
# Results
res_lstm_ConfirmedCases = show_lstm(forcast_ConfirmedCases, train_rate, lstm_size, days_num, forcast_ConfirmedCases.columns.values[0])

2.for stock close price prediction, just open stock_LSTM.ipynb
  make sure data directory is populated as well
3.data directory contains all the .csv files that needed by stock_LSTM.ipynb 
