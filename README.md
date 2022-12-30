# Neural Network Charity Analysis

## Overview of the analysis
The purpose of this analysis was to use deep learning neural networks and TensorFlow in Python to create a binary classifier that will be able to predict whether charity organization applicants would be successful if funded by Alphabet Soup. 

## Results
### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
  - The target variable for this model was the column IS_SUCCESSFUL because it represented whether or not the charity donation was used successfully.
- What variable(s) are considered to be the features for your model?
  - The variables considered features of the model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.
- What variable(s) are neither targets nor features, and should be removed from the input data?
  - The variables EIN and NAME were dropped because they did not provide any useful data for the model.


### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - We first created a model with two hidden networks. The first layer consisted of 80 neurons and the second of 30 neurons. We also included an output layer. For the activation functions, the hidden layers used “relu” and the output layer used “sigmoid”. 

![image1]([link](https://github.com/DaniliukK95/neural_network_charity_analysis/blob/main/images/image1.png))

- Were you able to achieve the target model performance?
  - In the module, the model was designed not to reach the target model performance. In the three attempts that I had performed, I could also not reach the performance of 75% or greater. 
- What steps did you take to try and increase model performance?
  - In my first attempt to increase performance, I only began with adding more neurons. I went from 80 and 30 in the first and second layer respectively, to 100 and 30 instead.

![image2]([link](https://github.com/DaniliukK95/neural_network_charity_analysis/blob/main/images/image2.png))

- In my second attempt I added more hidden layers and neurons to the model. I had 110, 50 and then 20 neurons in the first, second and third layers respectively.

![image3]([link](https://github.com/DaniliukK95/neural_network_charity_analysis/blob/main/images/image3.png))

- In my final attempt, I kept the previous settings for hidden layers but now changed the activation functions for all the hidden layers from “relu” to “tanh”.

![image4]([link](https://github.com/DaniliukK95/neural_network_charity_analysis/blob/main/images/image4.png))

## Summary
In my three attempts to increase the performance of the model, I was able to achieve: 72.9%, 73% and 72.6% accuracy for attempt 1, 2 and 3 respectively. Some more potential changes that could have been made to the model would be adjusting the input data. For example, we could have dropped more columns or even decreasing the number of values for each bin. Again, a different mix of the number of neurons and hidden layers could also help. To take a different approach, a different model such as the Random Forest model could prove useful since it is ideal for classification problems. This model also has a faster performance than the neural networks which could avoid overfitting data.
