The inspiration for creating a sign language detector comes from the desire to make communication more accessible and inclusive for the deaf and hard-of-hearing 
community. Sign language is a rich and complex language that uses hand gestures, facial expressions, and body language to convey meaning. 
However, not everyone is able to understand or use sign language, which can create barriers to communication and limit access to information. By developing a 
machine learning model that can recognize sign language, we can help bridge this communication gap and make it easier for people to connect 
with each other regardless of their hearing abilities. This technology has the potential to improve the quality of life for millions of people 
around the world, and represents a powerful example of how technology can be used for social good.

# What it does #

This sign language detector is a technology that uses machine learning algorithms to recognize and interpret sign language. The detector works by analyzing video 
data of a signer performing different signs and gestures and using this information to identify and interpret the meaning of the signs. The dataset will be used to 
train the machine learning model to recognize different signs and gestures. The dataset should include a variety of signers, lighting conditions, camera angles, 
and backgrounds to ensure the model is robust and can accurately detect signs in different settings. Next, the dataset is labeled, and the machine learning model is 
trained using a supervised learning approach. Once the model has been trained, it can be tested using a separate dataset to evaluate its accuracy. Finally when it's
properly trained, it can detect signs in real-time. It is even intergrated with voice-system so that it can read the sign and says the translated statement.

# How this is Built #
1. Importing all the required libraries
2. Collect keypoint values 

![nig(1)](https://user-images.githubusercontent.com/104302578/230726741-d80a8415-590e-4b05-8926-cd68cdcbfbf6.jpg)






3. Preprocess the collected data
4. Building and Training a LSTM neural network using oneAPI
5. Evaluating using confusion matrix
6. Save the model and test it

# Using oneAPI #

![intel-oneapi-cross-architecture](https://user-images.githubusercontent.com/104302578/230728549-12a0f722-d5d6-4815-9337-03094fe19545.png)


Using OneAPI for this project has several benefits. those are mentioned below:
1. Accelerated Performance: Sign language detection requires analyzing large amounts of visual data. OneAPI provides optimized libraries
   and frameworks that can take advantage of the hardware resources to accelerate the processing of this data and improve the performance of the model.
2. Scalability: Sign language detection requires training models with large datasets, which can be challenging on a local machine. OneAPI provides a scalable     solution that can distribute the workload across multiple nodes, making it easier to train large models and process large datasets.

model trained in local machine and in oneAPI:

![w1(2)](https://user-images.githubusercontent.com/104302578/230729137-8da40196-41c6-4ed7-9083-0a1ad8805d5d.jpg)
![w2(2)](https://user-images.githubusercontent.com/104302578/230729138-c1a79d63-8719-43e7-8489-ee5aa54e2597.jpg)




as we can see above, there is a good difference in accuracy score. This shows a good exploit of oneAPI.

# Dependencies Used #
1. Tensorflow
2. openCV - for computer vision
3. Mediapipe - for extracting keypoints
4. sklearn - for evaluation matrix and training the model
5. matplotlib - for visuvalizing images 

# Real time detection #

![sat(1)](https://user-images.githubusercontent.com/104302578/230734207-1e22a517-a04d-42e9-94d3-84dc52d89d1c.jpg)

with the trained model in oneAPI, we can get the model to the local machine and detect signs in real time.

------------------------

By leveraging the power of machine learning and oneAPI, we can create technology that can improve communication accessibility for the deaf and hard-of-hearing community. While there are challenges to overcome, the potential benefits of this technology make it a worthwhile endeavor.


