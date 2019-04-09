# human-or-not
Model showing if an image is human or not

Datasets - I have used the dataset 'horses and humans' which is availaible in tensorflow datasets.

Code - I have written this code using the google collabs kernels.

First of all the zipped file is unzipped and then the 4 directories having training and validataion data of humans and horses.
total training horse images: 500, total training human images: 527, total validation horse images: 628, total validation human images: 655. Some image visualization is done using matlplotlib library.

Model used - I have used the sequential model which takes 256x256 sized inputs. It has 5 convolution layers (3x3 filters) along with 2x2 maxpooling. Then model is compiled to use the 'rmsprop' optimizer and Binary crossentry as the loss.

Preprocessing - Preprocessing of image using image data generator. 

Training the images - Using model.fit_generator() to fit the training set and validating the validataion set, setting the epoachs to 10 and steps per epoachs to 8.

Accuracy - The accuracy for training set was 0.9854 and that for the test set comes out to be 0.9704.

Now just to see if an Image is human or not, I have uploaded the photo of Geoffrey Hinton and the model predicted correctly as human.


