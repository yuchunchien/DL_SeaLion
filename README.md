# DL_SeaLion
Final project for "Deep Learning for Computer Vision, Speech, and Language"
1. Project titile: Animal Population Calculation

2. Project Description: 
The primary goal of this project is to distinguish and count sea lions of the same species from different genders and ages (adult males, subadult males, adult females, juveniles, and pups). To track the population of animals, bioscientists would take pictures of the animals with a drone, identify all the animal in each picture, and calculate the amount of them. However, identifying animals is an arduous and time-consuming task. Thus, we propose a more efficient method for bioscientists to obtain the population from images. 
Our project takes images of sea lions as input and provides the counting results. The images taken by drones were provided by NOAA Fisheries Alaska Fisheries Science Center. The sea lions in the images were most likely lying in the sand or on the rocks, which have similar colors of sea lions'. Thus, it is not an easy task to identify them. It is an object identification project, but is different from ILSVRC, since we identify, instead of different species of animals, a particular kind of animal of different genders and ages.

3. File Description:

a) Crop_test_image.ipynb: Crop original pictures as fixed-sized images. The default size of the cropped image is 416*416.

b) bad_id.txt: Ids of the raw images which have problems.
