## Neural_Network_Charity_Analysis

## Overview Of The Analysis

Machine Learning and Neural Networks methods were used in the dataset to create a binary classifier that will help to predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful. For the analysis the dataset consisted on various measures of 34,000 organizations that have been funded by Alphabet Soup. 

The project is composed by the next 3 steps:

- Preprocessing the data for the neural network
- Compile, Train and Evaluate the Model
- Optimizing the model

## Results 

### Data Proccessing 

- Variable that was considered as the target for the model: IS_SUCCESSFUL Column
- Variables that were considered features for the model: Every Column asides for IS_SUCCESSFUL which is the target and the ones that will be dropped
- Variable that were neither targets or features for the dataset: Columns that were dropped are EIN, NAME since they won't have any effects on the model 

### Compiling, Training and Evaluating the Model

Number of neurons, layers, and activation functions selected for the neural network model:

For the neural network model 2 hidden layers were selected. First layer had 80 neurons, the second has 30 plus an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M1.png)

Did the model achieved the target model performance?

The model was not able to reach the target 75%. The accuracy for my model was 55%.

![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M2.png)

Steps to Improve the model 

Attempt 1: Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same. Accuracy improved to 69%

![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M3.png)
![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M4.png)

Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy decreased, this time it was 53%.

![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M5.png)
![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M6.png)


Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model decreased even more to 47%

![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M7.png)
![alt text](https://github.com/ramonmhung/Neural_Network_Charity_Analysis/blob/main/Resources/M8.png)

## Summary 

Model accuracy score was not to the standard with neural networks, using Random Forest classifiers would have been a better idea. The reason of this is that random forest is a robust and accurate model due to their sufficient number of estimators and tree depth. It's also possible to attest that random forest models provide a faster performance in comparison to neural networks and also the data could have not been overdrifted.





