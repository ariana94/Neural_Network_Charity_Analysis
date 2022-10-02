# Neural_Network_Charity_Analysis

## What's the Stitch?
In this project, we assisted Alphabet Soup in analzying data from their past 34,000 donations. We used deep-learning neural networks with TensorFlow in Python to classify and analyze the success and identify the predictors of donations. The goal of this project is to utilize input data housed in a historical spreadsheet to determine whether future applicants for chartiable organizations will be successful.


## Preprocessing the Data

- What variable(s) are considered the target(s) for your model?
  - The "IS_SUCCESSFUL" column was out target because it conatained binary data telling us if the donation was used successfuly.

- What variable(s) are considered to be the features for your model?
  - There are several: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT". Most of these columns had to be transformed because they were object data types.

- What variable(s) are neither targets nor features, and should be removed from the input data?
  - We removed "EIN" and "NAME" because it was just identification info and was not useful to this analysis.


## Compiling, Training, and Evaluating the model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - I chose to have two hidden layers with 80 (because this is almost twice the amount of input data) and 30 neurons. ReLu was used for the hidden layers and Sigmoid was used for the output layer. ReLu was chosen because it can handle the complex dataset in the most efficient way.

- Were you able to achieve the target model performance?
  - After numerous attempts, the closest I was able to get was 73%

- What steps did you take to try and increase model performance?
  - I tried dropping another column, changing the classification numbers, adding a hidden layer (I played around with other activation functions too), and tried different amounts of neurons and epochs.
  
## Summary
With the time I had on this project, I was not able to achieve 75% accuracy with the auto optimizer. It is possible that removing more outliers and finding that sweet spot of hidden layers and neurons would yield better results. I would also suggest trying supervised learning with Random Forest Classifiers to see if that can generate a higher accuracy using its multiple decision trees.

