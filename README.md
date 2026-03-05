🧠 House Price Prediction using Artificial Neural Networks (ANN)

📌 Project Overview

This project implements a Deep Learning model using Artificial Neural Networks (ANN) to predict house prices based on various housing features.

The objective of this project is to understand how neural networks can be applied to regression problems and how data preprocessing, feature scaling, and neural network architecture affect model performance.

This project was developed as part of my AI/ML interview preparation and Deep Learning learning journey.

📊 Dataset Information

The dataset contains housing information with the following features:

Feature       	Description
bedrooms	      Number of bedrooms
bathrooms     	Number of bathrooms
floors	        Number of floors
sqft_living	    Living area square footage
sqft_lot	      Lot size
waterfront	    Waterfront property indicator
view	          Property view rating
condition      	House condition
yr_built      	Year house was built
price	          Target variable (House Price)


⚙️ Technologies Used

Python
Pandas
NumPy
Scikit-Learn
TensorFlow
Keras

🧠 Deep Learning Concepts Applied

This project covers the following core neural network concepts:

Artificial Neural Networks (ANN)
Neurons, Weights and Bias
Activation Functions (ReLU)
Forward Propagation
Loss Functions
Optimizers (Adam)
Dropout (Overfitting Reduction)
Feature Scaling

🔄 Project Workflow

1️⃣ Data Loading

The dataset was loaded using Pandas.

2️⃣ Data Preprocessing

Selected important numerical features

Removed unnecessary columns

Applied log transformation on house prices to handle skewness

3️⃣ Train-Test Split

The dataset was divided into training and testing sets.

80% Training Data  
20% Testing Data

4️⃣ Feature Scaling

Used StandardScaler to normalize input features before training the neural network.

🏗 Model Architecture

Artificial Neural Network built using TensorFlow/Keras.

Input Layer
   ↓
Dense Layer (64 neurons, ReLU)
   ↓
Dropout Layer (0.2)
   ↓
Dense Layer (32 neurons, ReLU)
   ↓
Output Layer (1 neuron)
⚙️ Model Configuration
Parameter	Value
Optimizer	Adam
Loss Function	Mean Squared Error
Metric	Mean Absolute Error
Epochs	50
Batch Size	32

📊 Model Performance

After training the model, the performance on test data:

Test MAE ≈ 0.59 (Log Scale)

Predictions were converted back to the original price scale using:

np.expm1(predictions)

📌 Key Observations

ANN was able to learn relationships between house features and price.

Log transformation helped stabilize training.

Using only a few features reduced prediction accuracy.

Adding more features like sqft_living, location, and condition could improve model performance.

🚀 Future Improvements

Use more relevant features

Apply Feature Engineering

Try deeper neural networks

Compare ANN with ML models like:

Random Forest

Gradient Boosting

XGBoost

🎯 Learning Outcome

Through this project I gained hands-on experience with:

Deep Learning model building

Neural network architecture design

Regression problems using ANN

TensorFlow/Keras implementation

👩‍💻 Author

Anjali Chatla

AI / ML Enthusiast
Currently preparing for AI/ML Engineer roles
