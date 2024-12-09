# Facial-Recognition-AI
## Followed this Youtube tutorial: https://www.youtube.com/watch?v=bK_k7eebGgc&list=PLgNJO2hghbmhHuhURAGbe6KWpiYZt0AMH
## Discription
### Created a siamese model that can identify the similarity between two faces with high accuracy. The siamese model consists of two different models, one that analyzes each images and another that interprets the similarity between the values returned by the first model.
## Technologies Used
### Keras, Saimese model, Python
## Original Idea
### Originally to make a facial recognition model I planned to use a neural network attatched to a VGG16 model and train it like so
### -Run the model on one face from each person in the dataset
### -Set the label for all faces of a person as the value returned by the model
### -Repeatedly reset the labels between epochs until the model could distinguish between different people
### However, the model ended up not working and took a very long time to train.
## Differences Between the models
### -Data: In the Saimese model, the model was mainly trained using pictures I took from myself. This meant that there were a lot more similar images in the dataset, which increased the chance of two faces being similar. This prevents the model from always guessing that two images are different and getting the answer mostly right. 
### -Function: My original idea is similar to the first model of the Saimese model in that they both aim to analyze images and return similar values for similar images. However, my original idea was too ambitious in trying to compile the information from each image into one number. The Saimese model fixes this by combining the information from the model into multiple numbers, and using a seperate model to interpret the distance.
