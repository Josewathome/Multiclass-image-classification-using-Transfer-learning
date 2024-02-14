# PYTHON PROGRAMMING USING pre-trained model **InceptionResNetV2**, and customizing it.
## Multiclass image classification using Transfer learning
Image classification is one of the supervised machine learning problems which aims to categorize the images of a dataset into their respective categories or labels.
So, I have to classify more than one class that’s why the name multi-class classification
**Necessities for transfer learning**: Low-level features from model A (task A) should be helpful for learning model B (task B).

**InceptionResNetV2**: InceptionResNetV2 is a convolutional neural network that is 164 layers deep, trained on millions of images from the ImageNet database, and can classify images into more than 1000 categories such as flowers, animals, etc. The input size of the images is 299-by-299.

### Dataset Description.
The dataset used comprises of 120 breeds of dogs in total. here is the data : https://drive.google.com/drive/folders/1z31bsh7gNrUiwameOEWhqtWNZuKEdKQ7?usp=sharing 
Each image has a file name which is its unique id.
  - Train dataset ( train.zip ): contains 10,222 images which are to be used for training our model
  - Test dataset (test.zip ): contains 10,357 images which we have to classify into the respective categories or labels.
  - labels.csv: contains breed names corresponding to the image id.
  - sample_submission.csv: contains correct form of sample submission to be made

### For better performance Will be using GPU in Google.colab.
Because of the limited time one can use the free GPU in Colab I had to cut down the time for training.
so as to achive this and be able to train the model and evaluate it, I had to reduce the number of classes and number of images in the data set frim  10,222 to  5149 images and the classes from 120 to 60 this was done randomly.By doing this i was able to utilize the GPU in colab and was able to train and test the model which had an accuracy of 91.5% 


