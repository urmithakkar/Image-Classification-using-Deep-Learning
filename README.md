# Image Classification using Deep Learning

For this image classification task I've used the **Fashion-MNIST Dataset** and classified images into 10 categories using deep learning.

## Overview of the model:

▶ An architecture to process images based on **Multilayer Perceptrons**.

▶ Model architecture consists of Stem, Backbone and Classifier.

▶ The model is trained and evolution curves are analysed.
    
    ↪️ The curves for evolution of loss.
    
    ↪️ The curves for evolution of training and validation accuracies.
    
    ↪️ Hyper-parameter tuning.
    
 ## Hyper parameter tuning:
 
In my model, I have experimented with several hyperparameters such as,

1️⃣ Learning rate: It decides whether the network converges to the global minima or not.
I have used values like 0.01 , 0.05 , 0.001 , 0.005 in my experimentation but found
0.01 to be the best for my model.

2️⃣ Optimizers: It modifies the attributes of the neural network. I have experimented
with two optimizers, AdamOtimizer and SGD. After several experiments I can
conclude that AdamOptimizer worked best for my model.

3️⃣ Loss Function: It quantifies the difference between the expected outcome and the
outcome produced by the neural network. I have used two loss functions to
experiment with my model, NLLLoss() and CrossEntropyLoss(). For my model,
NLLLoss() worked the best.

4️⃣ Batch Size: It is thenumber of samples processed before the model is updated. I used
three batch sizes in my experimentation, 64 , 256 and 512. Batch size of 256 worked
the best.

5️⃣ Number of Epochs: It is the number of complete passes through the training dataset.
I have used 10, 20, 30 and 50 epochs in my model.

6️⃣ Activation Functions: Activation Functions map the non-linear functional inputs to
the outputs. These are highly important and right activation functions can boost the
model accuracy. I used three activation functions to experiment with my model, Relu,
Sigmoid and Tanh. The ReLU activation function worked best for my model.


## Final Model Accuracy on Fashion-Mnist Validation Set:

▶️ The final loss and accuracy are:
Training loss: **0.26036026940700857** 

Train Accuracy **90.41** 

Test Accuracy **87.33**


## Loss and Accuracy Curves for the Final Model Accuracy:

![image](https://user-images.githubusercontent.com/62324786/177370851-5292dbe5-21ef-43ea-82a9-b70a26b2f5f2.png)
