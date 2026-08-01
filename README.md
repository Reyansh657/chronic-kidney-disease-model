# Chronic-kidney-disease-model

  This project uses 2 models, *random forest* and *convulsional neural network*, whilst using UC Irvine's dataset *336*. This is the *chronic kidney disease* datset, 
Rivaan coded the *random forest* whilst Reyansh did the *convulsional neural network*. Later on a comparision of the model will be shown.
# Goal and what we want to acomplish from this project
Our project intially was very different in terms of what we trying to do., we were planning on making models for different data sets. However Mr.Miyata suggested that instead we try to make multiple models for one dataset, then we make a comparision between the models to see which was better on the dataset. So we moved on from our previous idea where we were working on the MNIST data set (Reyansh and Joshua) aswell as the CKD (Rivaan) and began to focus on just the CKD (*Chronic Kidney Disease*). Since Josh didn't say for the remaining final week, Rivaan and Reyansh took on the task of making their own individual model for the dataset. Since Rivaan had already started on a *Random Forest* model for the dataset, Reyansh began to work on a *Convolusional Neural Network* for the dataset. Essnetially, our projects goal was to find the best model for the UCI *Chronic Kidney Disease* dataset.
# How it works
The Random forest splits up the main dataset into random smaller pieces so each tree gets a slight different set of data to practice on. When the trees are growing, they only look at a random mix of features at each step. This keeps the trees different from each other so they do not all make the exact same mistakes.

# Finding the answer
* For picking categories (classification) every single tree in the forest votes on what they think the answer is. The model picks whichever choice got the most votes.
* For figuring out numbers (regression) every tree guesses a number. The model just takes the average of all those numbers for the final answer

# Why we chose random forest
* It does not overfit as easily as a single decision tree since the average of a lot of trees cleans up the bad gueeses.
* It tells you feature importance, which means it shows you which parts of your data actually mattered the most for the final guess.
* It is easy to use on a normal data tables and you do not even have to spend a ton of time cleaning or scaling your numbers first.

# Explaining the models - Convulsional  Neural Network
Our 2cd model was CNN, convolutional neural network. We will start of with a description on a neural network, a neural network which consists of 3 layers, the input (raw data inputed by the user), hidden layer (calculations, activation functions (Like ReLU), etc.), and output layer(returns out the prediction/result). Remembering the fact that CNN is a type of neural network, that clearly implies and means that it also has  similar networking to those of a typical neural network.
### Convulsional
In the beginning convolutional layer, CNN uses a kernel (filter) which is "slid" across the data array, which could be typically of 1 to 3 dimensions. The kernel filter helps detect patterns by detecting and alyzing the data looking for local patterns and sequences. The kernel filter looks through the data array as it analyzes the dataset looking for local patterns it also beings to search for feature matrices, feature maps. These features maps are certain sections of the data, each of these features maps will be used for a step of linear transformation. Before this step is done, using a theorem regarding the sigma sum method in order to create a calculated matrix. The feature map is then multiplied by the calculated matrix, know that each feature amtrix is multiplied by the same matrix. Each feature map on the page is replaced by the product of it and the matrix on the page.
#### Activation Function
After the convolution operation, an activation function is applied to introduce non-linearity into the model. This allows the network to learn more complex patterns instead of just linear relationships.
A typical activation function is ReLU (Rectified Linear Unit), which replaces negative values with 0 while keeping positive values unchanged. This helps the model focus on important features, introducing non-linearity with non-linear functions while increasing efficiency and helping learn more complex patterns.

### Pooling
Pooling is used to reduce the size of the feature maps while preserving important information. This helps in the models learning, accelrating it by removing extra noise which could overwhelm the learning rate for the model only pserserving the signifcant data and information
The most common type is max pooling, which takes the maximum value from a small region (we used a 2×2 pool size area). This keeps the most important features, while reducing the unnecessary data helping keep only what is signficant removing anything nose data to overwhelm the model.
### Fully connected
In the fully connected layer, the feature maps are flattened into a single vector and passed through one or more dense layers.
Each neuron is connected to all values from the previous layer, allowing the network to combine all learned features and make a final prediction.

# *Comparision*

In conclusion, we can cleraly see the random forest was abetter model than CNN in terms of its predicting ability and accuracy.
