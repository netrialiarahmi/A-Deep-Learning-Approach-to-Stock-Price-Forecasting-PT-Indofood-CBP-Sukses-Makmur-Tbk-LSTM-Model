# A-Deep-Learning-Approach-to-Stock-Price-Forecasting-PT-Indofood-CBP-Sukses-Makmur-Tbk-LSTM-Model
This repository contains code for implementing an LSTM model to predict stock prices for PT Indofood CBP Sukses Makmur Tbk. The model is trained on historical stock prices and can be used to make predictions for future prices.

The Long Short-Term Memory (LSTM) algorithm is a type of Recurrent Neural Network (RNN) that is widely used for processing time series data. LSTM is particularly effective in handling complex issues in time series data such as nonlinear trends, repetitive patterns, and long-term interactions between variables in the dataset.

The primary function of the LSTM algorithm in time series data is to predict future values. LSTM is capable of identifying patterns and trends in time series data and using them to estimate future values. As a result, LSTM is widely used for various prediction applications, including stock price prediction, weather prediction, and sales prediction.

LSTM is also used for time series data analysis, including identifying outliers, correlation between variables, and short-term and long-term forecasting. In this regard, LSTM can help stakeholders make better business decisions based on accurate and reliable time series data analysis.

Overall, LSTM is a powerful algorithm that can effectively process complex time series data and provide accurate and reliable prediction results. Therefore, LSTM has become a popular choice for practitioners and researchers who want to analyze and predict time series data.

## There are several reasons why we use this model:
1. LSTM Model: LSTM is a type of Recurrent Neural Network (RNN) algorithm specifically designed to process time series data. LSTM can handle issues in time series data such as nonlinear trends, repetitive patterns, and long-term interactions between variables in the dataset. Therefore, LSTM is a good choice for predicting time series data.

2. Sequential Model: Keras.Sequential() is an easy way to create a deep learning model by linking a series of layers sequentially. In this case, we create an LSTM model by adding LSTM and Dense layers.

3. Input Shape: LSTM requires input in the form of three dimensions (number of data, timestep, number of features). Therefore, we need to specify the input_shape as (x_train.shape[1], 1) to adjust the input data dimensions.

4. LSTM Layers: In the above code, we add two LSTM layers with 100 neuron units and return_sequences=True in the first layer. Return_sequences=True is used to specify that the first LSTM layer outputs in a three-dimensional format, so the output can be used as input for the next LSTM layer.

5. Dense Layers: After the two LSTM layers, we add two Dense layers. Dense layers are responsible for mapping the output from the LSTM layer to the final prediction.

6. Model Summary: We can use model.summary() to see the structure of the model we have created and make sure that everything is connected correctly.

## notes
In the model.compile(optimizer='adam', loss='mean_squared_error') section, we specify the optimizer that will be used to adjust the model weights and the loss function used to measure the model's prediction error. Adam is one of the popular optimizers in deep learning, and mean_squared_error is the loss function used to calculate the difference between the model's predicted value and the actual value in the data.

Next, in the model.fit(x_train, y_train, batch_size=1, epochs=3) section, we train the model by providing training data (x_train and y_train). batch_size determines the number of samples used in each iteration when training the model, while epochs determine how many times the model will see the entire training data. The more epochs, the longer it takes to train the model.

 If the data used is larger, we usually use a larger batch_size to speed up the training time.

## Conclusion of this analysis
The conclusion of this analysis is that the root mean squared error (RMSE) for this prediction model is very small, at 1.2976633707682292, indicating that the error of the predictions is very low. This result suggests that the LSTM model with the specified parameters is an effective method for predicting stock prices.
