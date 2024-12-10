#### Facial-Recognition-AI
## Welcome to the Facial Recognition AI project! 
#### This AI model aims to use Siamese Neural Networks and the VGGFace model to recognize and compare faces in images, and integrate with real-time camera detection. The techniques I used in this project followed ideas from this Youtube [tutorial](https://www.youtube.com/playlist?list=PLgNJO2hghbmhHuhURAGbe6KWpiYZt0AMH).
## Technologies Used
- Keras, Saimese model, Python
## This is an Ongoing Project
I am still working on this project for better accuracy!
## Description
The facial recognition system uses a Siamese Neural Network designed to learn the similarity between pairs of faces. The Siamese model consists of two key components:
- Feature Extraction Model: Processes each image to extract meaningful features (e.g., using a VGG16-based architecture).
- Similarity Model: Compares the extracted features from both images and determines their similarity. </br>

I planned to use a neural network attatched to a VGG16 model and iteratively refining the labels to improve the model's ability to distinguish between individuals. 
 - Run the model on one reference face for each person in the dataset
 - Set a consistent label to all faces of the same person based on the model's output
 - Repeatedly reset and refine the labels between training epochs until the model achieves robust discrimination between different individuals.
 - This iterative approach ensures that the model adapts to better accuracy over time. And I am still working on this process.
## Lessons Learned from This Project
 - Data: In the Siamese model, most of the training data consisted of pictures I took of myself. This created a dataset with a higher proportion of similar images, which helped address a common issue: the model defaulting to always predicting that two images are different. By including more similar pairs in the dataset, the model was encouraged to learn nuanced features and make more accurate distinctions. This approach significantly improved its performance in identifying genuinely similar images.
 - Function: My original idea shared similarities with the first stage of the Siamese model, as both aimed to analyze images and produce similar outputs for similar images. However, I soon realized that my initial approach was overly ambitious in attempting to condense all the information from an image into a single numerical value. The Siamese model addresses this limitation by encoding the image's features into a multi-dimensional representation. It then utilizes a separate model to interpret the distance between these feature representations, making the comparison process more robust and effective.  I am now revising my model to follow a two-step algorithm and incorporating a larger database for training. 
