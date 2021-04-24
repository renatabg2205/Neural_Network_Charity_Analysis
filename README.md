# Neural_Network_Charity_Analysis

## Overview of the analysis:

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Explain the purpose of this analysis.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

## Results:
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Using bulleted lists and images to support your answers, address the following questions.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

### Data Preprocessing

- What variable(s) are considered the target(s) for your model?

The column "IS_SUCCESSFUL" was considered the target for this model. It contains information whether the money was used effectively or not.

- What variable(s) are considered to be the features for your model?

The columns "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT" are considered to be the features for this model.

- What variable(s) are neither targets nor features, and should be removed from the input data?

"EIN" and "NAME" are identification columns and were removed from the input data.


### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

This neural network model has two hidden layers: one has 80 neuros and the other has 30 neurons.
The activation functions are relu and sigmoid.

![Neurons, layers and activation functions](./Images/image1.PNG)

- Were you able to achieve the target model performance?

The target model performance was not achieved because the target predictive accuracy was lower than 75%.

![Accuracy](./Images/image2.PNG)

- What steps did you take to try and increase model performance?

In order to try to increase model performance a different activation function was used, however, the target model performance was not achieved.

![Different activation function: tanh](./Images/image3.PNG)

![Second attempt accuracy](./Images/image4.PNG)

Another attempt was made by adding a third hidden layer but the target predictive accuracy was lower than 75%.

![Adding a third hidden layer: tanh](./Images/image5.PNG)

![Third attempt accuracy](./Images/image6.PNG)

we applied bucketing to the feature ASK_AMT and organized the different values by intervals.
We increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.
We also tried a different activation function (tanh) but none of these steps helped improve the model's performance.

For the trial to improve the accuracy of the model three layers were added and the number of neurons was increased as noted in the images below. I found that adding layers did not improve the accuracy, rather it stayed the same about 72%. For my last attempt I removed the third layer and increased the neurons to 200 for the first layer and 80 for the second layer. I increased the neurons for each attempt because there was a larger distribution of data points with in each feature.


## Summary: 
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!