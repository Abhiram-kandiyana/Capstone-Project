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
In this project I am going to classify whale species by looking at the pictures of their tails.The dataset contains nearly 25,000 images of different whales' tails images which should be large enough for the model to be trained.I believe I can achieve a decent score using transfer learning from one of those benchmark models for ImageNet data classification.The problem is simple.We need to first be able to detect the whales'tails from the given images using OpenCV.and then classify them to the given labels

In this section, clearly describe the problem that is to be solved. The problem described should be well defined and should have at least one relevant potential solution. Additionally, describe the problem thoroughly such that it is clear that the problem is quantifiable (the problem can be expressed in mathematical or logical terms) , measurable (the problem can be measured by some metric and clearly observed), and replicable (the problem can be reproduced and occurs more than once).

### Datasets and Inputs
The inputs are nothing but the images of the whales' tails.Some of these might needed to be preprocessed so that all the images are of the same dimensions.The dataset is gathered by happywhale and can be downloaded from kaggle.Their usage is perfectly appropriate as the data has been given for competetions in kaggle.The dataset is used as an input for the model.

In this section, the dataset(s) and/or input(s) being considered for the project should be thoroughly described, such as how they relate to the problem and why they should be used. Information such as how the dataset or input is (was) obtained, and the characteristics of the dataset or input, should be included with relevant references and citations as necessary It should be clear how the dataset(s) or input(s) will be used in the project and whether their use is appropriate given the context of the problem.

### Solution Statement
(approx. 1 paragraph)
The solution to this problem is simple.I would use transfer learning from on of the beest models out there and some fully connected  layers on the end .
In this section, clearly describe a solution to the problem. The solution should be applicable to the project domain and appropriate for the dataset(s) or input(s) given. Additionally, describe the solution thoroughly such that it is clear that the solution is quantifiable (the solution can be expressed in mathematical or logical terms) , measurable (the solution can be measured by some metric and clearly observed), and replicable (the solution can be reproduced and occurs more than once).

Benchmark Model
(approximately 1-2 paragraphs)
As this is one of the most recent problems I don't think I can have a very good be
In this section, provide the details for a benchmark model or result that relates to the domain, problem statement, and intended solution. Ideally, the benchmark model or result contextualizes existing methods or known information in the domain and problem given, which could then be objectively compared to the solution. Describe how the benchmark model or result is measurable (can be measured by some metric and clearly observed) with thorough detail.

Evaluation Metrics
(approx. 1-2 paragraphs)
I believe accuracy score would be the best evaluation metric for  this project.The accuracy of the image to be a certain whale is calculated and is compared to its original label.Based upon the overall results the accuracy for the model is given.

In this section, propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms).

Project Design
(approx. 1 page)
I would start my project by importing all the important libraries like openCV,os
In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project.

Before submitting your proposal, ask yourself. . .

Does the proposal you have written follow a well-organized structure similar to that of the project template?
Is each section (particularly Solution Statement and Project Design) written in a clear, concise and specific fashion? Are there any ambiguous terms or phrases that need clarification?
Would the intended audience of your project be able to understand your proposal?
Have you properly proofread your proposal to assure there are minimal grammatical and spelling mistakes?
Are all the resources used for this project correctly cited and referenced?
