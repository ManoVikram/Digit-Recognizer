# Deigit Recognizer

This is a Kaggle contest to learn computer vision fundamentals with the famous MNIST data.

Link: [Digit Recognizer](https://www.kaggle.com/competitions/digit-recognizer/overview)

## Given dataset

The data files train.csv and test.csv contain gray-scale images of hand-drawn digits, from zero through nine.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. The rest of the columns contain the pixel-values of the associated image.

## Approach

Built a CNN model with 2 convolutional layers with 64 and 128 filters each of size 3x3. 2x2 Max pooling is done. The final dense layers has 256 neurons with 'relu' activation function. The final output layer has 10 neurons depicting 10 differnt classes to predict from 0 to 9 with 'softmax' activation function.

#### Note
I just doubled all the vlaues (number of neurons) to improve the accuracy by 0.001% which in this case is not necessary. The model will give 99% accuracy even with half the neurons.