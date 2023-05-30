# DeepLearning projects overview



----------------------------
#1. MNIST using CNN
----------------------------
The MNIST dataset is known as the get go dataset for deep learning beginners. This dataset is used for handwritten digits classification. I implemented Convolutional Neural Network on this MNIST dataset, with 2 convolutional layers (with Relu activation function), 2x2 max pooling and 2 fully connected layers to train the model. I used 11 epochs which gave the final accuracy result as 98.280% on the test dataset and took 20 minutes to train, with a learning rate of 0.001 and a momentum of 0.9, on the Stochastic Gradient Decent optimizer. 

----------------------------
#2. F-MNIST using CNN, Regularization
----------------------------
This is also a famous classification for beginners. Modelled on the MNIST dataset, this dataset enables classification of fasion items like shoes on the basis of the images. Just like MNIST, I have used the Convolutional Neural Network. This time, I have performed data augmentation by giving slight changes on images' shape, colour, skew etc. I also applied Batch Normalization on the first and second layer, used L2 Regularization with a weight_decay of 0.001 and a droupout rate of 0.2. The model gave an accuracy of 89.78 percent and took 22 minutes to train.

-----------------------------
#3. Visualization using GradCAM and its variations
------------------------------
GradCAM basically takes the feature maps produced by the output layer of CNN, adds differentiable layers to get the gradients, and weight the feature maps using the alpha values achieved from the gradients. This makes a heatmap, which is then overlaid on the image to visualise what deep learning actually sees. Also multiple variations to it were used- <br>
1. GradCAM++ - Provides better visualization<br>
2. ScoreCAM - Gradient free method. Time taking Visualization. cuda GPUs recommended.<br>
3. FasterScoreCAM - Quicker visualization than ScoreCAM<br>
Used tensorflow coupled with keras, for the minority of the syntaxes, on a pretrained ImageNet dataset utilising the 16-layered VGG-16 convolutional model. 
