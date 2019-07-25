# logistic_regression
In statistics, the logistic model is used to model the probability of a certain class or event existing such as pass/fail,
win/lose, alive/dead or healthy/sick. This can be extended to model several classes of events such as determining whether
an image contains a cat, dog, lion, etc...
Consider a scenario where we need to classify whether an email is spam or not. 
If we use linear regression for this problem, there is a need for setting up a threshold based on which classification can be done.
Say if the actual class is malignant, predicted continuous value 0.4 and the threshold value is 0.5,
the data point will be classified as not malignant which can lead to serious consequence in real time.
From this example, it can be inferred that linear regression is not suitable for classification problem.
Linear regression is unbounded, and this brings logistic regression into picture. Their value strictly ranges from 0 to 1.


MNIST data:
The data files train.csv and test.csv contain gray-scale images of hand-drawn digits, from zero through nine.

Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. 
Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel,
with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. 
The rest of the columns contain the pixel-values of the associated image.
Each pixel column in the training set has a name like pixelx, where x is an integer between 0 and 783, inclusive.
To locate this pixel on the image, suppose that we have decomposed x as x = i * 28 + j, where i and j are integers between 0 and 27,
inclusive. Then pixelx is located on row i and column j of a 28 x 28 matrix, (indexing by zero)
