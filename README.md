# Final-Project---ECE-697ML

# Extrapolation of CNN Trained on Mars Satellite Data to Classify Lunar Features
### Aniruddha Prasad, Andrew Hartnett

## Project Description:
For this project, we will be using two different data sets. One will be a set of orbital images of Mars that have already been labeled. This dataset has been obtained from the Mars Reconnaissance Orbiter and will be used to train the model. We then plan to implement transfer learning to tweak our trained model to classify images from a second dataset that contains images of the lunar surface. This second dataset is obtained from the Lunar Orbiter Gallery.
We are aiming to see how well transfer learning will help in classification of images from a completely different astronomical body.

## Data Set Description:
Training dataset: Mars Orbital HiRISE image data set - This data set contains a total of 73,031 landmarks. 10,433 landmarks were detected and extracted from 180 HiRISE browse images, and 62,598 landmarks were augmented from 10,433 original landmarks. For each original landmark, we cropped a square bounding box that includes the full extent of the landmark plus a 30-pixel margin to left, right, top and bottom. Each cropped landmark was resized to 227x227 pixels, and then was augmented to generate 6 additional landmarks using the following methods:
  A. 90 degrees clockwise rotation
  B. 180 degrees clockwise rotation
  C. 70 degrees clockwise rotation
  D. Horizontal flip
  E. Vertical flip
  F. Random brightness adjustment

## Testing/Implementation dataset: 
The Lunar Orbiter Photo Gallery is an extensive collection of over 2,600 high- and moderate-resolution photographs produced by all five of the Lunar Orbiter missions. These photographs were taken in 1966 and 1967 to survey possible lunar landing sites and provide baseline imagery for geologic analysis of the lunar surface. The images were used to select the Apollo landing sites and to produce many of our existing lunar geologic maps. This photo gallery is the web’s most comprehensive collection of Lunar Orbiter photography and supporting documents. For our implementation, we plan to label a subset of these images to conduct transfer learning and testing.

## Algorithms to be implemented:
In a similar fashion to the “Deep Mars” paper associated with the HiRISE dataset, we plan to train a Convolutional Neural Network (CNN). We have considered also implementing a Random Forest Classifier on the same HiRISE dataset as a benchmark model for the CNN. This will give us a chance to explore an advanced neural network that is new for us to learn as well as reference a known algorithm in the process. To apply our trained model from Mars satellite data to Lunar satellite data, we will also need to conduct transfer learning.

## Programming Environments to be used:
For this task, Python with TensorFlow to train our neural network and conduct transfer learning. Training of the benchmark Random Forest Classifier would be done solely with Python as well. We also will be making use of popular libraries such as scikit-learn, pandas, and numpy for data manipulation. Initial exploration into the tools has shown we will also be making use of the Keras API to implement the neural network.

## Data Set Links:

Lunar Orbiter Dataset
HiRISE Mars Satellite Dataset
