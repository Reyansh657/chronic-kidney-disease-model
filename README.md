# Chronic-kidney-disease-model

  This project uses 2 models, *random forest* and *convulsional neural network*, whilst using UC Irvine's dataset *336*. This is the *chronic kidney disease* datset, 
Rivaan coded the *random forest* whilst Reyansh did the *convulsional neural network*. Later on a comparision of the model was made to explore which of the 

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

Our 2cd model was CNN, convolutional neural network. We will start of with a description on a neural network, a neural network which consists of 3 layers, the input (raw data inputed by the user), hidden layer (calculations, activation functions (Like ReLU), etc.), and output layer(returns out the prediction/result). Remembering the fact that CNN is a type of neural network, that clearly implies and means that it also has  similar networking to those of a typical neural network. In the beginning convolutional layer, CNN uses a kernel (filter) which is “slid” across to detect and analyze local/common patterns in the input data, the input data grid collected by the kernel is multiplied by a calculated matrice. For our specific code we converted the data into a 1D array which was multiplied by a matrix which was 1D aswell. Following that, an activation function is used, typically will be the ReLU function, this helps in the learning of more complex patterns. Afterwards, is a pooling layer, this is when a shrinking method is used to get remove of data which is not necceasry and significant in order to help in the mpodel learning and keeping important values to help the model not sensitive to change. Finally comes the fully connected layer, which is the final layer where a final prediction is made and returned. 
# as
