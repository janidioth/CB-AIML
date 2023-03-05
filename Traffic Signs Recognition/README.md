# Deep Learning with Keras and TensorFlow
# Traffic Signs Recognition

## DESCRIPTION
Self-driving cars are the future as people can entirely depend on the car for traveling.

In the world of AI, many researchers and big companies like Tesla, Google, Mercedes-Benz, Toyota, Ford, and Audi are working on self-driving vehicles and cars. To achieve accuracy with this technology, vehicles need to understand and follow the traffic rules accordingly.

There are many types of traffic signs, such as no parking, speed limit, no-entry, turn left or right, school ahead, no honking, and so on.

## Objective: 
To create a model that can accurately distinguish between distinct traffic signals from photos using a Convolutional Neural Network

## Dataset Details: 
The dataset contains three folders and two Excel files, which are:

* **Train folder:** This folder has a subfolder with a class label as its name, and the sub-folder has images related to the class that can be used for training the model.
Extract 'Train.zip' to a 'data' folder and all other 'Train1.zip' to 'Train9.zip' into the /data/Train folder.

* **Test folder:** It has 12631 images that should be used to evaluate the model.
Extract 'Test.zip' to a 'data' folder and 'Test1.zip' and 'Test2.zip' into the /data/Test/ folder.

* **Sample images for classes:** It has one image of each class in high definition for illustration purposes.

* **Train_data_label Excel file:** This file has the class Id of all the images in the train folder along with its path.

* **Test_data_label Excel file:** It has the path/name of the images in the test folder along with its class label.

**There are more than 50000 images of 43 traffic signs, which are:**  
**0:** Speed limit (20km/h)  
**1:** Speed limit (30km/h)   
**2:** Speed limit (50km/h)   
**3:** Speed limit (60km/h)     
**4:** Speed limit (70km/h)   
**5:** Speed limit (80km/h)   
**6:** End of speed limit (80km/h)   
**7:** Speed limit (100km/h)   
**8:** Speed limit (120km/h)   
**9:** No passing   
**10:** No passing vehicle over 3.5 tons   
**11:** Right-of-way at the intersection   
**12:** Priority road   
**13:** Yield   
**14:** Stop   
**15:** No vehicles   
**16:** Vehicle > 3.5 tons prohibited   
**17:** No entry   
**18:** General caution   
**19:** Dangerous curve left   
**20:** Dangerous curve right   
**21:** Double curve   
**22:** Bumpy road   
**23:** Slippery road   
**24:** Road narrows on the right   
**25:** Road work   
**26:** Traffic signals   
**27:** Pedestrians   
**28:** Children crossing   
**29:** Bicycles crossing   
**30:** Beware of ice/snow  
**31:** Wild animals crossing   
**32:** End speed + passing limits   
**33:** Turn right ahead   
**34:** Turn left ahead   
**35:** Ahead only   
**36:** Go straight or right   
**37:** Go straight or left   
**38:** Keep right   
**39:** Keep left   
**40:** Roundabout mandatory   
**41:** End of no passing   
**42:** End no passing vehicle > 3.5 tons 

**Steps to be followed:** 
* Import the required libraries
* Read the Train_data_label Excel file
* Read the images in the train folder and resize them to 30 X 30
* Create a NumPy array from the resized images
* As the image is still in RGB format, it can be converted to grayscale
* For the other columns in the data, save the image's color image array in a new column named color_img_arr
* For the other columns in the data, save the grayscale image array of images in a new column named grayscale_img_arr
* Plot the bar chart of classes from the train and test data by replacing the numbers with actual class names in the graph
* Prepare the model's training and testing data, as well as convert the labels and data to the format or shape required by the model

**Create two CNN models, one with color images and the other with greyscale images, using the following steps:**   

**Note:** use Keras library
* Add Convolutional, MaxPool, and DropoutLayers
* Use Relu as an activation function
* Take the loss function as binary cross-entropy
* Take Adam as an optimizer
* Use early-stop with two patients and monitor for validation loss
* Experiment with the five epochs
* Refine the CNN model color images until an accuracy of 90% or more is achieved by different filter shapes, neurons, activation functions, optimizers, and architecture
* Plot the training and validation accuracy for color and grayscale models
* Observe the precision, recall the F1-score for all classes for both grayscale and color models, and determine if the model's classes are good 
* Compare the color and grayscale CNN models and analyze which model is better
