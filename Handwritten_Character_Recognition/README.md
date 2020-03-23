### **Capstone Project**

The aim of this project is to predict the characters of the handwritten Telugu words.  
Following are the key stages,

##### Identification of the problem

Voice and character recognition are one of the most complex topics in data science as we continue to digitize human life everyday. Many researchers have built models to solve these complex problems. In an attempt to test my capabilities in data science techniques, I decided to pursue my capstone project on character recognition to identify handwritten Telugu characters.

##### Acquiring Data

A dataset comprising of over 120K handwritten words is made available by a research group in International Institute of Information Technology (IIIT), Hyderabad in India. Mode details of the dataset are available at https://cvit.iiit.ac.in/research/projects/cvit-projects/indic-hw-data 

##### Parse, Mine & Refine the data

This stage of the project has most number of steps,
	Cleansing the image
		read the image using image package 
		convert the image to black and white
		remove the noise in the image by manipulating the pixel data
	Find the cluster of the pixels within image to identify each character
	merge or split clusters to make appropriate characters
	identify position of each character to be able to construct the word after each character prediction
	standardize the resultant characters
	convert the pixel matrix into a data row
	split the target word label into character labels
	associate the character data point with the corresponding character label
	split data 80-20 to train and test the models respectively
	

##### Build a data model

At this stage following models are trained using train data and tested the accuracy score using test data
	Logistic Regression
	Decision Trees 
	Bagging with Decision trees
	Random forests
	Bagging with Logistic regression
	Neural networks with TensorFlow

##### Results

​	Model that gave best accuracy score: Logistic regression with regularisation
​	Baseline Score: 0.08365098066394068
​	Best accuracy score: 0.574984180552626 (Mean CV)
​	

##### Conclusion

​	Handwritten character recognition is one of the complex issue and there is lot of scope to improve as the current models available are not generalized enough.
​	Prediction inconsistencies can be analysed to find exactly where the model is failing which may help to identify additional features required to improve the score
​	Additional layer of modelling can be done at word level to predict correct word even when some of the characters are predicted incorrectly
​	Thickness of the letters can be minimized to bring down the size of the training data