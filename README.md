Dataset Link:- http://mrl.cs.vsb.cz/eyedataset

Data Preparation has been updated with train and test folder split automation.
In the dataset, we annotated the following properties (the properties are indicated in the following order):
subject ID; in the dataset, we collected the data of 37 different persons (33 men and 4 women)
image ID; the dataset consists of 84,898 images
gender [0 - man, 1 - woman]; the dataset contains the information about gender for each image (man, woman)
glasses [0 - no, 1 - yes]; the information if the eye image contains glasses is also provided for each image (with and without the glasses)
eye state [0 - closed, 1 - open]; this property contains the information about two eye states (open, close)
reflections [0 - none, 1 - small, 2 - big]; we annotated three reflection states based on the size of reflections (none, small, and big reflections)
lighting conditions [0 - bad, 1 - good]; each image has two states (bad, good) based on the amount of light during capturing the videos
sensor ID [01 - RealSense, 02 - IDS, 03 - Aptina]; at this moment, the dataset contains the images captured by three different sensors (Intel RealSense RS 300 sensor with 640 x 480 resolution, IDS Imaging sensor with 1280 x 1024 resolution, and Aptina sensor with 752 x 480 resolution)

An examples of image annotations of the proposed dataset:

![image](https://user-images.githubusercontent.com/75678695/138558051-138d7285-ded8-4ce3-98c2-52627a0a1e1f.png)




The example images from this dataset of open and closed eyes are shown below.

![image](https://user-images.githubusercontent.com/75678695/138558125-28c71382-ab7e-4562-a62a-d44a699ff6d6.png)




To obtain eye images, we used the eye detector based on the histogram of oriented gradients (HOG) combined with the SVM classifier. The eye images presented in the proposed dataset can be used to train the eye detector. Examples of eye detection are shown in the following images.

![image](https://user-images.githubusercontent.com/75678695/138558156-46fcd06e-5c07-4fe8-b3dd-1445cb07e63f.png)



