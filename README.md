# Hand-signs-dataset

# Introduction

The dataset format is patterned to match closely with the classic MNIST. Each training and test case represents a label (0-25) as a one-to-one map for each alphabet letter A-Z (and no cases for 9=J or 25=Z because of gesture motions). The training data (27,455 cases) and test data (7172 cases) are approximately half the size of the standard MNIST but otherwise similar with a header row of label, pixel1,pixel2....pixel784 which represent a single 28x28 pixel image with grayscale values between 0-255. The original hand gesture image data represented multiple users repeating the gesture against different backgrounds.
But it is difficult to perform machine learning alogorithm's on the images so we have to convert the images in the form of csv file. For that we have to compress the images to represent each images in the form of pixel.There are 28X28 pixels in one image.<br>
Each pixel has a specific value. So our final dataset will be the pixel representation of the image.

# Objectives

<li>View the data as an image</li><br>
<li>Train different classifiers</li><br>
<li>Compare performance for different classifiers using various metrics</li>

# Dataset

The dataset is in the form of a csv file:<br>
https://drive.google.com/file/d/1cbu3KfAXXmqVrWNTuHhK7uQTh70xv7Mk/view?usp=sharing/

# Dataset description

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255. The training and test data sets have 785 columns. The first column consists of the class labels (see above), and represents the article of clothing. The rest of the columns contain the pixel-values of the associated image.
<li>To locate a pixel on the image, suppose that we have decomposed x as x = i * 28 + j, where i and j are integers between 0 and 27. The pixel is located on row i and column j of a 28 x 28 matrix.</li>
