# Final-Project---ECE-697ML

# Comparison of CNN to Vision Transformer Model Trained on HiRISE Mars Satellite Images
### Aniruddha Prasad, Andrew Hartnett

## Project Description:
For this project, we will be using two state-of-the-art models popular for image classification tasks, the Convolutional Neural Network (CNN) and Vision Transformer (ViT). We use the "Deep Mars" paper from Wagstaff et al. as our inspiration to determine if the Transformer architecture, which was only recently applied for image classification tasks in 2020, could be better suited for the task of classifying Mars satellite images instead of the CNN originally used in the work. We train both model and draw comparisons between the two, as well as look at how changing parameters like pre-training dataset and batch size of the Transformer trainer effect its testing accuracy.
We are aiming to see if the newly applied Transformer architecture can outperform a CNN used on the HiRISE dataset from the "Deep Mars" paper.

## Data Set Description:
Mars Orbital HiRISE image data set - This data set contains a total of 73,031 landmarks. 10,433 landmarks were detected and extracted from 180 HiRISE browse images, and 62,598 landmarks were augmented from 10,433 original landmarks. For each original landmark, we cropped a square bounding box that includes the full extent of the landmark plus a 30-pixel margin to left, right, top and bottom. Each cropped landmark was resized to 227x227 pixels, and then was augmented to generate 6 additional landmarks using the following methods:
- 90 degrees clockwise rotation
- 180 degrees clockwise rotation
- 70 degrees clockwise rotation
- Horizontal flip
- Vertical flip
- Random brightness adjustment

## Algorithms to be implemented:
In a similar fashion to the “Deep Mars” paper associated with the HiRISE dataset, we plan to train a Convolutional Neural Network (CNN). We will also be implementing several variations of a Vision Transformer (ViT) model in attempts to outperform the CNN. This will give us a chance to explore a known algorithm to us in the form of a custom CNN while seeing how a new model like the Transformer can be implemented.

## Programming Environments to be used:
For this task, Python with TensorFlow to train our neural network and conduct transfer learning. The HugsVision wrapper used for training the ViT model runs on PyTorch, which will be used indirectly. All code will be conducted within a Jupyter Notebook (HiRISE_Model_Analysis.ipynb).

## Data Set Link:
HiRISE Mars Satellite Dataset - https://data.nasa.gov/Space-Science/Mars-orbital-image-HiRISE-labeled-data-set-version/egmv-36wq
