## Computer Vision Project: Emotion Recognition

### DESCRIPTION
Future customizations, such as understanding human emotions, could lead to a range of advancements, such as determining whether a person likes a specific statement, item or product, food, or how they are feeling in a particular circumstance, and so on. 

### Objective:
To build a model using a convolutional neural network that can classify a person's emotion

### Dataset description:
The dataset contains two folders named Train and Test. These folders have approximately 35,000 images of seven different human emotions, such as anger, disgust, fear, happiness, neutral, sadness, and surprise.

**Train folder:** This folder has images for training the model, which is divided into subfolders having the same name as the class. 

**Test folder:** This folder has images for testing the model, which is divided into subfolders having the same name as the class.

#### **Following operations should be performed using KERAS or PyTorch or Torch vision:**  
1. Import the necessary libraries
2. Plot sample images for all the classes 
3. Plot the bar graph for the number of images in each class for both training and testing data
4. Build a data augmentation for train data to create new data with translation, rescale and flip, and rotation transformations. Rescale the image at 48x48
5. Build a data augmentation for test data to create new data and rescale the image at 48x48
6. Read images directly from the train folder and test folder using the appropriate function

### Build 3 CNN model with: 
1. **CNN Architecture:**
    1. Add convolutional layers, max pool layers, dropout layers, batch normalization layers  
    2. Use Relu as activation functions
    3. Take loss function as categorical cross-entropy
    4. Take Adam as an optimizer
    5. Use early-stop with two patiences and monitor for validation loss
    6. Try with ten number epochs
    7. Train the model using the generator and test the accuracy of the test data at every epoch
    8. Plot the training and validation accuracy, and the loss
    9. Observe the precision, recall the F1-score for all classes for both grayscale and color models, and determine if the model’s classes are good
    
2. **Customized CNN Architecture:**
    1. Add convolutional layers, max pool layers, dropout layers, batch normalization layers on the top of the first model architecture to improve the accuracy
    2. Change the batch size activation function and optimizer as rmsprop and observe if the accuracy increases
    3. Take the loss function as categorical cross-entropy
    4. Use early stopping with the patience of two epochs and monitoring of validation loss
    5. Try with ten number epochs
    6. Train the model using the generator and test the accuracy of the test data at every epoch
    7. Plot the training and validation accuracy, and the loss
    8. Observe the precision, recall the F1-score for all classes for both grayscale and color models, and determine if the model’s classes are good
    
3. **Transfer Learning:**
    1. Prepare the data for the transfer learning algorithm 
    2. Freeze the top layers of the pre-trained model     
    3. Add a dense layer at the end of the pre-trained model followed by a dropout layer
    4. Add the final output layer with the SoftMax activation function
    5. Take the loss function as categorical cross-entropy
    6. Take Adam as an optimizer
    7. Use early stopping with the patience of two epochs and monitor the validation loss which is set as minimum mode
    8. Try with fifteen number epochs
    9. Train the model using the generator and test the accuracy of the test data at every epoch
    10. Plot the training and validation accuracy, and the loss
    11. Observe the precision, recall the F1-score for all classes for both grayscale and color models, and determine if the model’s classes are good

### Final Steps:
1. Compare all the models on the basis of accuracy, precision, recall, and f1-score
2. Write at least 3 more things to increase the model’s performance

