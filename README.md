# Final project for "Deep Learning for Computer Vision and NLP"
## Project titile: 
Animal Population Calculation

## Project Description: 
The primary goal of this project is to distinguish and count sea lions of the same species from different genders and ages (adult males, subadult males, adult females, juveniles, and pups). To track the population of animals, bioscientists would take pictures of the animals with a drone, identify all the animal in each picture, and calculate the amount of them. However, identifying animals is an arduous and time-consuming task. Thus, we propose a more efficient method for bioscientists to obtain the population from images. 
Our project takes images of sea lions as input and provides the counting results. The raw images taken by drones were provided by NOAA Fisheries Alaska Fisheries Science Center. The sea lions in the images were most likely lying in the sand or on the rocks, which have similar colors of sea lions'. Thus, it is not an easy task to identify them. It is an object identification project, but is different from ILSVRC, since we identify, instead of different species of animals, a particular kind of animal of different genders and ages.

## File Description:
1. Crop_test_image.ipynb: Crop original pictures as fixed-sized images. The default size of the cropped image is 416*416.

2. bad_id.txt: Ids of the raw images which have problems.

3. parse_files.ipynb: Generate localization ground truth for training with different options. Although locations of each sea lion in the raw images have been labeled with dots, the range of each sea lion was not defined. Since the range is essential for training object identification algorithms, we define two types of generating criteria for localization ground truth, fixed-sized square and growing-sized rectangle.

Fixed-sized square criterion estimates the range with a square of size D*D. The default values of D are 32 and 64. 

Growing-sized rectangle criterion initially estimates the range with a rectangle of size E*E. Then, augment along the direction of the edge with a similar color of the middle of the rectangle. The default values of E are 16 and 32.

4. remove_bad_image.ipynb: Eliminate raw images with problems from training data set.

