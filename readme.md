**Description**

A deep neural network regression model was created to predict the Tomatometer and 
audience ratings of movies. A dataset of over 17,000 movies as preprocessed and used to train 
this model. Information such as runtime, content rating, actors, authors, directors, release month, 
and production company was either One-Hot encoded (categorical variables) or normalized 
(continuous variables). The model was four layers deep with an input layer of 240 nodes, two 
hidden layers of 64 nodes, and an output layer of 1 node. ReLu was the activation function of 
choice, except for the output node which used a linear activation function. The resulting model 
had a 15.22% mean absolute error when predicting audience rating and a 21.46% mean absolute 
error when predicting Tomatometer rating. The model was able to make low accuracy 
predictions for movie ratings

**Model**

![image](https://user-images.githubusercontent.com/65905153/190724153-2c465e27-4925-43b7-8077-644a501f6728.png)

For the model itself, it is a four-layer neural 
network. The first layer, the input layer, has 240 
nodes and a ReLu activation function. There are then 
two 64 node hidden layers also with ReLu activation. 
Finally, the output layer is 1 node with a linear 
activation function

**Results**
![image](https://user-images.githubusercontent.com/65905153/190724451-eb17c3bc-b504-45ba-a0d3-21fad65e1a50.png)
The results were varied depending on whether we were predicting on the audience score 
or the Tomatometer score. The audience score had a mean absolute error of 15.22% and showed 
some non-random predictions when compared to the true score. However, the Tomatometer 
rating had a mean absolute error of 21.46% and showed no significant predictions. This was 
likely due to a large amount of 0% true ratings that were fed into the model.
