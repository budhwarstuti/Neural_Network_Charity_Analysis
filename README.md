# Neural_Network_Charity_Analysis

## **Overview of the analysis**
The purpose of the project is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Following steps were taken in the process:
* Preprocessing Data for a Neural Network Model
* Compile, Train, and Evaluate the Model
* Optimize the Model

## **Results**
**Data Preprocessing**
* I used "Is_successful" column as target for my model.
* The features for my model were columns like Apllication_Type, Bin, Income etc. These are the independent variables which are the input for our model.
* EIN and Name the 2 columns that are neither targets nor features, and were removed from the input data.

**Compiling, Training, and Evaluating the Model**
* In the main section, I used  an input layer, a hidden, an output layer. Also I used "Relu" for input and "Sigmoid" activation function for my output layer in neural network model. This provided an accuracy of about 73%.

* Steps taken to try and increase model performance were as follows:

* 1st Optimization attempt- Here I tried to adjust the input data to ensure that there are no variables or outliers that are causing confusion in the model by dropping columns. I dropped 3 columns, AFFILIATION_CompanySponsored, SPECIAL_CONSIDERATIONS_N, SPECIAL_CONSIDERATIONS_Y and the accuracy fr the model went down to 53% implyinh my decision was incorrect. I dropped AFFILIATION_CompanySponsored column which shouldnt have been done and badly effected the model accuracy.
* 2nd Optimization attempt- Here I tried adding another hiden layer to my model. This gave an accuracy of 72.7% which is very close to the accuracy attained with the original model. 
* 3rd Optimization attempt- Here I chnaged the activation function of the input layers from "ReLu" to "tanh". This gave an accuracy of 72.86% which is agian very close to the original model.

* Despite trying 3 of the optimizaton techniques as mentioned above, I was not able to achieve the target model performance of 75%. 


## **Summary**
Even after multiple optimization techniques applied to the model, the accuracy did not meet the targeted rate and was pretty consistent implying this was the best the model could do in terms of accuracy.