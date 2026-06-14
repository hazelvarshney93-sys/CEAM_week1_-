# CEAM_week1_- DESK OBJECT CLASSIFIER

This is a simple demonstration of a machine learning model, which classifies which hotwheels car I have on my desk.

For this project, the dataset was required to be custom made. I took around 20-25 photos of each of my 3 hotwheels in order to make this dataset.
The photos were taken in different lighting conditions, different locations and different angles in order for our machine learning model to be as
efficient as possible.

The first issue I encountered was the file size. My model was taking around 5 minutes to scan one full dataset. I decided to compress the images to 300x300 pixels
in order to fix this problem.

The second issue issue was underfitting, where I was only using 10 epochs because the dataset I was using previously was too large. I turned up the epochs to 50 and
it gave much more accurate results. Also at the same time reducing the batch size from 32 to 8.

The third and the biggest issue I encountered was that my model gave the same output no matter what image I uploaded. This was because I was using an Artifical Neural Network instead of a Convolutional Neural Network. An ANN seemed to work fine for the MNIST database model but the problem with it was that it was destroying the overall spatial structure of the pictures. What a CNN does better is that it does not flatten the image. It keeps the image as is and slides small filters across it, which in the end gave much more accurate results. I have attatched all of those scenarios alongwith their graphs.

I have also attatched the custom dataset for this project. I have also attatched some more pictures I took of my hotwheels that are not included in my dataset, so you can test it on your own.
