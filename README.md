# **Churn Prediction using Artificial Neural Networks (ANN)**  

## **Project Overview**  
This project uses an Artificial Neural Network to predict customer churn in a bank. The model analyzes key customer attributes such as credit score, age, number of products, and account balance to determine whether a customer is likely to leave the bank.  

## **Dataset**  
The dataset used in this project is `Churn_Modelling.csv`, which contains customer information, including:  
- **Credit Score**  
- **Geography**  
- **Gender**  
- **Age**  
- **Tenure**  
- **Balance**  
- **Number of Products**  
- **Has Credit Card**  
- **Is Active Member**  
- **Estimated Salary**  
- **Exited (Target Variable: 1 = Churn, 0 = Retained)**  

## **Project Steps**  

### **1. Data Preprocessing**  
- Load the dataset using Pandas  
- Encode categorical variables (Label Encoding and One-Hot Encoding)  
- Scale the features using StandardScaler  
- Split the data into training and test sets  

### **2. Building the ANN**  
- Create a Sequential model using TensorFlow/Keras  
- Add two hidden layers with ReLU activation  
- Add an output layer with a sigmoid activation for binary classification  
- Compile the model using Adam optimizer and binary cross-entropy loss  

### **3. Training the Model**  
- Train the ANN on the training dataset for 50 epochs with a batch size of 32  

### **4. Making Predictions**  
- Predict churn for a new customer  
- Evaluate model performance using a confusion matrix and accuracy score  
