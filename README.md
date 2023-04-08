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
trained using a supervised learning approach. Once the model has been trained, it can be tested using a separate dataset to evaluate its accuracy. Finally when its
properly trained, it can detect signs in real-time. It is even intergrated with voice-system so that it can read the sign and says the translated statement.

# How this is Built #
1. Importing all the required libraries
2. Collect keypoint values 
3. Preprocess the collected data
4. Building and Training a LSTM neural network using oneAPI
5. Evaluating using confusion matrix
6. Save the model and test it

# Using oneAPI #
Using OneAPI for a sign language detection project can have several benefits. those are mentioned below:
1. Accelerated Performance: Sign language detection requires analyzing large amounts of data, including visual and audio data. OneAPI provides optimized libraries
   and frameworks that can take advantage of the hardware resources to accelerate the processing of this data and improve the performance of the model.
2. Scalability: Sign language detection requires training models with large datasets, which can be challenging on a local machine. OneAPI provides a scalable solution 
   that can distribute the workload across multiple nodes, making it easier to train large models and process large datasets.
