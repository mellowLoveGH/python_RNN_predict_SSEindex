# RNN_predict_SSEindex
Quantify the Shanghai Composite Index (000001.SS),  preprocess the close index of each day, and then use a simple RNN (recurrent neural network) to learn  the internal relationship of the time series, finally predict the index for the next day.   对上证指数进行量化，对每天的收盘指，进行一个基本的处理，然后用简单的RNN循环神经网络去处理，和学习时间序列的内部关系，然后预测下一天的指数。

tools: pandas, datdaframe, series, yfinance (yahoo finance)
用的主要包为：pandas, datdaframe, series, yfinance (yahoo finance)

here some simple neural networks are used: 
1. MLP, dense
2. SimpleRNN
1 model based on MLP, 3 on RNN
Totally, there are 4 simple models used to predict.
这里主要用到4个简单模型，分别是全连接层，和RNN
其中有3个是RNN。

For the preprocess, just calculate the MV(moving average) and EMA(exponential moving average) based on close index of each day.
Use EMA as the feature to train models, every window is 20 size, about one month (about 20 days every month there is stock open)
对于金融量化方面，主要是用 移动平均数 （滑动平均数）， 基本的和指数类型的来处理每天的收盘点数
一个月，一般是20多天的开盘，所以计算移动平均数 （滑动平均数）用的窗口大小是20

Quantify the Shanghai Composite Index (000001.SS),  
preprocess the close index of each day, 
and then use a simple RNN (recurrent neural network) to learn  the internal relationship of the time series, 
finally predict the index for the next day.  

 对上证指数进行量化，
 对每天的收盘指，
 进行一个基本的处理，
 然后用简单的RNN循环神经网络去处理，
 和学习时间序列的内部关系，然后预测下一天的指数。



