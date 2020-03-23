### **Capstone Project**

The aim of this project is to predict the characters of the handwritten Telugu words.  
Following are the key stages,

##### Identification of the problem

Voice and character recognition are one of the most complex topics in data science as we continue to digitize human life everyday. Many researchers have built models to solve these complex problems. In an attempt to test my capabilities in data science techniques, I decided to pursue my capstone project on character recognition to identify handwritten Telugu characters.

##### Acquiring Data

* A dataset comprising of over 120K handwritten words is made available by a research group in International Institute of Information Technology (IIIT), Hyderabad, India. 
* Details of the dataset are available at, https://cvit.iiit.ac.in/research/projects/cvit-projects/indic-hw-data 

##### Parse, Mine & Refine the data

This stage of the project includes EDA and Preparation of data for modelling. Following are the key points of this stage of the project

* Cleansing the image
  * Read the image using image package 
  * Convert the image to black and white
  * Remove the noise in the image by manipulating the pixel data
* Find the cluster of the pixels within image to identify each character
* Merge or split clusters to make appropriate characters
* Identify position of each character to be able to construct the word after each character prediction
* Standardize the resultant characters
* Convert the pixel matrix into a data row
* Split the target word label into character labels
* Associate the character data point with the corresponding character label
* Split data 80-20 to train and test the models respectively
  	

##### Build a data model

At this stage following models are trained using train data and tested the accuracy score using test data

* Logistic Regression
* Decision Trees
* Bagging with Decision trees
* Random forests
* Bagging with Logistic regression
* Neural networks with TensorFlow

##### Results

* Model that gave best accuracy score: Logistic regression with regularisation
* Baseline Score: 0.08365098066394068
* Best accuracy score: 0.574984180552626 (Mean CV)

##### Key challenges

* Splitting the characters from an image having a word of un-known length of characters is the most challenging task of this project
* Generalization of the train data as the hand writing varies from person to person
* Managing the size of the data points and predictors is another key aspect to be able to run the models in reasonable time frame

##### Conclusion & Future work

* Undoubtedly handwritten character recognition is one of the complex issues
* There is lot of scope to improve models by generalization of training data
* Prediction inconsistencies can be analysed to find short comings of the model which may help to identify additional features required to improve the accuracy score
* Additional layer of modelling at word level to predict correct word even when some of the characters are predicted incorrectly will help to improve the score further
* Thickness of the letters can be minimized to bring down the size of the training data
* Due to the time and resource constraints, support vector models are not tested in this project. However, from the research SVMs are the better models for HCR projects



Please refer presentation on the project for more detail of the project https://github.com/agksuman/DSI-Projects/blob/master/Handwritten_Character_Recognition/CapstoneProject_Suman_2020_at_GA.pdf