# Neural_Network_Charity_Analysis
 # Overview of the analysis:

The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.
We use the following methods for the analysis:

1.preprocessing the data for the neural network model,

2.compile, train and evaluate the model,

3. optimize the model.

# Results:
## Data Preprocessing

. The columns EIN and NAME are identification information and have been removed from the input data.

. The column IS_SUCCESSFUL contains binary data refering to weither or not the charity donation was used effectively. This variable is then considered as the target for our deep learning neural network.

. The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model.

. Encoding of the categorical variables, spliting into training and testing datasets and standardization have been applied to the features.

## Compiling, Training, and Evaluating the Model.

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

The output layer is made of a unique neuron as it is a binary classification.
To speed up the training process, we are using the activation function ***ReLU*** for the hidden layers. As our output is a binary classification, ***Sigmoid*** is used on the output layer.

## Here evaluate model using test data.

![Evaluate_mode-1)](/Resources/Evaluate_mode-1.png)

2.Were you able to achieve the target model performance?

The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.

![Testing_Data)](/Resources/Testing_Data.png)

3.What steps did you take to try and increase model performance?

![Hidden_layer)](/Resources/Hidden_layer.png)

We increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.But none of these steps helped improve the model's performance.

# Summary:

In summary, we present a deep neural network classification model that predicts loan applicant success from feature data contained in charity_data.csv with 72% accuracy. This does not meet the 75% accuracy target, and the optimization methods employed here have not caused significant improvement.

### Additional Optimization Methods
Performance could increase through additional optimization techniques such as visualizing the numerical feature variable ASK_AMT to find and remove potential outliers that could be causing noise. Additionally, one could iteratively tune the parameters above and keep optimal values when moving to subsequent parameters instead of reverting to the base setting and combining after completion. This would however require more careful thought on the order with which one adjusts parameters to arrive at an optimized model.
