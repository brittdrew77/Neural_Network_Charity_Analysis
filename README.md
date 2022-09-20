# Neural_Network_Charity_Analysis
## 1. Overview of the Analysis
The purpose of this analysis is to help predict successful investments for a company. I created a binary classifier that is able to determine whether applicants that are funded will be successful. I preprocessed a large dataset in order to then compile, train, and evaluate the neural network model. Lastly, I used various techniques to attempt to optimize the model and increase accuracy to 75%. 

## 2. Results
* Data Preprocessing
  * The target variable is the IS_SUCCESSFUL variable. This column is used to determine whether the money was used effectively.
  * The feature variables are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and SPECIAL_CONSIDERATIONS. 
  * The variables that were removed from the input data were EIN and NAME. They are identification variables and have no impact on the target variable.
* Compiling, Training, and Evaluating the Model
  * I used two hidden layers, the first with 80 neurons and the second with 30 neurons. I used two hidden layers, since it was the default and adding hidden layers is best for optimization. I used a lot of neurons, since there was a large data set. I used two different activation functions: relu and sigmoid. Relu was used for the hidden and input layers, since it is the most flexible. Sigmoid was used for output, since we want values between 0 and 1 to be able to classifiy a successful investment or not. 
  * After making various changes to optimize the neural network model, I was unsuccessful in reaching 75% accuracy. Although, I was able to slightly increase accuracy with my different attempts. 
  * I tried adding a hidden layer, increasing epochs, adding neurons to the hidden layers, and changing activation functions. 

## 3. Summary
Overall, I reached an accuracy of 73% which is not great for a neural network model, so further optimization would be needed for the model to be more accurate. There was also a large loss metric of 55%. I would recommend a random forest ensemble learning model. It is more interpretable and has a higher accuracy. It also handles outliers and nonlinear data very well. 
