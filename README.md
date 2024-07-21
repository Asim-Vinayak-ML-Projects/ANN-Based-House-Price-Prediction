# ANN-Based-House-Price-Prediction
# House Price Prediction using ANN

## Aim of the Project
The aim of this project is to predict house prices in India using an Artificial Neural Network (ANN). This model leverages various features from the dataset to make accurate predictions on house prices, which can be helpful for buyers, sellers, and real estate professionals.

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- TensorFlow
- Scikit-learn
- Matplotlib

## Dataset
The dataset used is `House Price India.csv`, which contains various features such as area type, availability, location, size, society, total_sqft, bath, balcony, and price.

## Methodology
1. **Data Preprocessing**:
   - Loading the dataset using Pandas.
   - Splitting the dataset into features (`X`) and target (`y`).
   - Splitting the data into training and testing sets.
   - Scaling the features using `StandardScaler`.

2. **Model Building**:
   - Defining an ANN model using TensorFlow's Keras API.
   - Adding input, hidden, and output layers to the model.
   - Compiling the model with an optimizer and loss function.
   
3. **Model Training**:
   - Training the model on the training data for 100 epochs.
   - Monitoring the training loss and mean absolute error (MAE) over epochs.

4. **Model Evaluation**:
   - Predicting house prices on the test data.
   - Visualizing the model's performance through various plots.

## Results
### Training Loss and MAE over Epochs
The training loss and mean absolute error (MAE) decrease over epochs, indicating the model is learning effectively.


![image](https://github.com/user-attachments/assets/2a550da2-a2c1-42d1-8d9b-b3c3236d062e)



### Actual vs Predicted House Prices
The scatter plot shows the actual vs predicted house prices, with a red dashed line representing the ideal prediction scenario.


![image](https://github.com/user-attachments/assets/5b6c0e92-b760-4494-b7a9-cdc2bfd30185)
## Line Plot: Actual vs Predicted House Prices

![image](https://github.com/user-attachments/assets/f3cd8b88-141d-4f6a-a54b-337358b0e0f5)


### Description
This line plot shows the actual house prices (in blue) and the predicted house prices (in orange) over a range of samples.

### Analysis
- The model seems to have a general upward trend in predictions similar to the actual house prices.
- However, the predicted values show significant noise and variability, especially for higher-priced houses.
- The discrepancy between actual and predicted values increases as the house prices increase, indicating that the model struggles with higher-priced houses.
- The closeness of the blue and orange lines in the lower price range suggests that the model performs better with lower-priced houses.

### Error Distribution Plot Analysis
![image](https://github.com/user-attachments/assets/2ce4b727-b0f0-47f8-9905-db9bee7bf8ce)

The error distribution plot is a crucial diagnostic tool for evaluating the performance of your house price prediction model. Here’s a detailed analysis of what the plot reveals about the model’s predictions:

#### Key Observations

1. **Centered Around Zero:**
   - The histogram shows that the majority of prediction errors are centered around zero. This indicates that the model's predictions are, on average, close to the actual house prices.

2. **Symmetrical Distribution:**
   - The distribution appears to be relatively symmetrical around the zero error mark. This symmetry suggests that the model does not consistently over-predict or under-predict the house prices, which is a desirable characteristic.

3. **Tight Spread:**
   - Most of the errors are within a narrow range around zero, indicating that the model’s predictions are generally accurate. However, there are some outliers with larger errors, which could be due to atypical data points or areas where the model could be improved.

4. **Presence of Outliers:**
   - There are some extreme values on both ends of the error spectrum. These outliers may indicate instances where the model struggled to make accurate predictions, possibly due to unusual property features or prices.

5. **Error Magnitude:**
   - The x-axis scale shows that most prediction errors fall within the range of -0.5e6 to 0.5e6. This range represents the deviation of predicted house prices from actual prices, with a larger concentration of errors close to zero.


## Analysis of Results
- The training loss decreases significantly, showing that the model is fitting well to the training data.
- The mean absolute error (MAE) decreases over epochs, indicating an improvement in model predictions.
- The scatter plot of actual vs predicted prices shows a strong positive correlation, demonstrating the model's effectiveness in predicting house prices accurately.

## Conclusion
This project demonstrates the use of an ANN for predicting house prices based on various features. The results show that the model can predict house prices with reasonable accuracy. Further improvements can be made by tuning hyperparameters, adding more features, or using more advanced neural network architectures.

## How to Run the Project
1. Clone the repository.
   ```bash
   git clone https://github.com/yourusername/House_Price_Prediction.git
