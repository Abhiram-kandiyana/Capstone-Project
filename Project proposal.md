# Machine Learning Engineer Nanodegree
## Capstone Proposal
Abhiram kandiyana

26th february, 2019

## HumpBack Whale Identification

### Domain Background
After centuries of intense whaling, recovering whale populations still have a hard time adapting to warming oceans and struggle to compete every day with the industrial fishing industry for food.
To aid whale conservation efforts, scientists use photo surveillance systems to monitor ocean activity. They use the shape of whales’ tails and unique markings found in footage to identify what species of whale they’re analyzing and meticulously log whale pod dynamics and movements. For the past 40 years, most of this work has been done manually by individual scientists, leaving a huge trove of data untapped and underutilized.
For science, unique identifiable markings on a whale's flukes (tail) and dorsal fin allow us to non-invasively track whale movements and stories over time. By focusing on whales, we bring attention to the marine ecosystem as a whole and the challenges we face as a global community.
Most large whale species were heavily exploited by whaling throughout their ranges. The primary method scientists use to measure population recovery is whale photo-identification. With sighting histories of individually recognizable whales, scientists can estimate population trends. As whale numbers have recovered from a century of intense hunting, and as photography-savvy whale watchers travel farther with better equipment, scientists have the potential to access an amazing amount of photographic samples.
I have always been interested in image classification and whales are one of my favourite animals.The greatest motivation is that I can actually help the latter by doing working with the former.
This project is an active competition in [kaggle]().I would like to thank [HappyWhale](https://happywhale.com/home) for putting their efforts to save these beautiful creatures and making this project possible.Happywhale is a platform that uses image process algorithms to let anyone to submit their whale photo and have it automatically identified.

### Problem Statement 
The problem statement is simple and clear.The model takes images as inputs and it needs to predict it's label. In this project I am going to classify whale species by looking at the pictures of their tails.The dataset contains nearly 25,000 images of different whales' tails images which should be large enough for the model to be trained.I believe I can achieve a decent score using transfer learning from one of those benchmark models for ImageNet data classification.The problem is simple.We need to first be able to detect the whales'tails from the given images using OpenCV's object detector.and then classify them to the given labels(ID's).

### Datasets and Inputs
The inputs are nothing but the images of the whales' tails.Some of these might needed to be preprocessed so that all the images are of the same dimensions.The dataset is gathered by happywhale and can be downloaded from kaggle.Their usage is perfectly appropriate as the data has been given for competetions in kaggle.
* train - contains all the images(25363)
* train.csv-a dataset which is a mapping between the image and its ID.
* test - contains all test images.We need to predict the id for the images.

### Solution Statement
The solution is to build a CNN architecture model for image classification.Using pretrained models like resenet50,Inceptionv3 would be better.applying a few number of fully connected layers at the end of the architecture must do the magic.I would use a softmax function on the last layer to differentiate different classes of images.Then train the data for 500 to 1000 epochs and test it for better accuracy.
In this section, clearly describe a solution to the problem. The solution should be applicable to the project domain and appropriate for the dataset(s) or input(s) given. Additionally, describe the solution thoroughly such that it is clear that the solution is quantifiable (the solution can be expressed in mathematical or logical terms) , measurable (the solution can be measured by some metric and clearly observed), and replicable (the solution can be reproduced and occurs more than once).

### Benchmark Model
I believe an accuracy score of 85% would be an amazing score.As this is an recent research I don't think I can find a benchmark model for this but like any image classfication model a good accuracy score would be enough to evaluate the solution.


### Evaluation Metrics

I believe accuracy score would be the best evaluation metric for  this project.The accuracy of the image to be a certain whale is calculated and is compared to its original label.Based upon the overall results the accuracy for the model is given.A test accuracy of 85% can be considered to be an amazing score.

### Project Design
I would start my project by importing all the important libraries like openCV,OS,keras,tensorflow,matplotlib.then I would import the images and the datasets.We need to implement the object-identifier from openCV.Generally any background like tensorflow takes a 4D image as input.the 4 dimensions are (n,224,224,3).Here n is the count of the samples remaing three are rows,columns,channels.and all the images must be resized into a square image of 224 X 224 pixels.As all the images are color the channel is three(red,green,blue) for all the images.We need a function to do the all the preprocessing which takes a array of images as input and gives the optimized array of images. The last step in preprocessing is to reorder RGB to BGR but as most of the pretrained models have this part in them we can leave it to them.Now we are gonna build a CNN for classifying the images.we would use pretrained models and add some fully connected layers at the end so that the model adapts to our image classification.Next the most important thing is to train the model with the training sample and test the model for good accuracy with the test samples.We need to keep changing parameters,implementing different supplementary function,make sure the model doesn't overfit.



