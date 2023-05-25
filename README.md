# Deep-learning-challenge

***Overview:*** The purpose of this module was to use various machine learning methods in predicting the chance of successfully getting funding for a new venture (not specified). The evaluation of each model's accuracy rates were first depended on the following process steps:

<ins>Data Processing:</ins>
* _Target Variable:_  <br>
Column labeled-Is_Successful: Noting 1 (Successful) and 0 (Failure). Labeled as y variable
* _Feature Variables:_ <br>
Application type, Affiliation, Classfiication, use-case, organization, status, income_amount, special consideration, asking amount. Labeled as X, with the removed of the target variable
* _Non useful variables:_ <br> EIN & Name, since they are classficaition or identifying datapoints that does not need to go into the model

<ins>Model setup:</ins> Compiling, Training, and Evaluating the Model <br>
There were three models that were tested manually through trial and error, along with a final tuner method. They are descibed below:

**_Model 1 Or Initial:_** [Model1-Notebook](https://github.com/djthapa22/deep-learning-challenge/blob/main/Initial%20Notebook/Deep_Learning.ipynb)
* How many neurons, layers, and activation functions did you select for your neural network model, and why? <br>
  * First Layer: Nuerons-10; Activation function: Relu
  * Second Layer: Neurons- 8; hidden function: Leaky Relu
  * Output Layer: Nueron- 1; Sigmoid layer with probability function
  * Rationale: Starting off at a base level with begining architechture with leaky and relu to see performance baseline
* Were you able to achieve the target model performance? <br> No, I was not able to acheive the 75% accuracy, since my accuracy rate was 72.93%
* What steps did you take in your attempts to increase model performance? <br> In the next model I was determined to increase the layers, neurons and even change the function type!

**_Model 2:_** [Model2-Notebook](https://github.com/djthapa22/deep-learning-challenge/blob/main/Initial%20Notebook/Deep_Learning.ipynb)
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  * Layers: 6 hidden layers and one output layer; Neurons: First and 6th had 50 neurons each, while 2nd through 5th had 25 layers; function: Activation to 6th layer had Tanh, while last one was sigmoid due to probabilitistic output
  * Rationale: I significantly increased the density of the architechture and wanted to see if Tanh would fare better.
* Were you able to achieve the target model performance? <br> No, I had an accuracy score of 72.69%, which was worse than my base line model.
* What steps did you take in your attempts to increase model performance? I wanted to further increase density of architechtrure and go back to Leaky_relu and Relu.


**_Model 3:_** [Model2-Notebook](https://github.com/djthapa22/deep-learning-challenge/blob/main/Initial%20Notebook/Deep_Learning.ipynb)
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
 * Layers: 9 hidden layers and one output layer; Neurons: All hidden had 250 function: Activation and 9th was Relu, while remaining was Leaky_Relu. Finally,the last one was sigmoid due to probabilitistic output
  * Rationale: I significantly increased the density of the architechture and thought a more complex neural network along with Relu/Leaky_Relu would get the numbers closer to 75%
* Were you able to achieve the target model performance? <br> No, I had an accuracy score of 72.37%, which was even worse than my base line model and Model 2.
* What steps did you take in your attempts to increase model performance? I learned that the complexity of the architecture may not be the solution and decided on using a tuner to find out the best way to get closest to the 75% mark!



**_Tuner Model:_**

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* Were you able to achieve the target model performance?
* What steps did you take in your attempts to increase model performance?


<ins> Summary:</ins>
