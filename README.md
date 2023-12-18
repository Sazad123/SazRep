# Faster RCNN for Human Detection

## Team Members are:
1) Sukanta Bala  
2) Sazad Alam Shah   
3) Md Hassanujjaman  
4) Baishakhi Sharma  

## What is Neural Network?  
A neural network is a method in artificial intelligence that teaches computers to process data in a way that is inspired by the **human brain**. 
It is a type of machine learning process, called deep learning, that uses interconnected nodes or neurons in a layered structure that resembles the human brain. 
It creates an adaptive system that computers use to learn from their mistakes and improve continuously. Thus, artificial neural networks attempt to solve 
complicated problems, like summarizing documents or recognizing faces, with greater accuracy.   

### What are Neural Network used for?    
There are many applications of Neural Networkss. Some of them are:    
#### 1) Computer Vision :
   Computer vision is the ability of computers to extract information and insights **from images and videos**. With neural networks, computers can distinguish and recognize images similar to humans. Computer vision has several applications, such as the following:
   * Visual recognition in self-driving cars so they can recognize road signs and other road users.
   * Content moderation to automatically remove unsafe or inappropriate content from image and video archives.
   * Facial recognition to identify faces and recognize attributes like open eyes, glasses, and facial hair.
   * Image labeling to identify brand logos, clothing, safety gear, and other image details.

#### 2) Speech Recognition :
   Neural networks can analyze **human speech** despite varying speech patterns, pitch, tone, language, and accent. Virtual assistants like Amazon Alexa and
   automatic transcription software use speech recognition to do tasks like these:
   * Assist call center agents and automatically classify calls.
   * Convert clinical conversations into documentation in real time.
   * Accurately subtitle videos and meeting recordings for wider content reach.

#### 3) Natural Language Processing :
   Natural language processing (NLP) is the ability to **process natural, human-created text**. Neural networks help computers gather insights and meaning from text data and documents. NLP has several use cases, including in these functions:  
   * Automated virtual agents and chatbots.
   * Automatic organization and classification of written data.
   * Business intelligence analysis of long-form documents like emails and forms.
   * Indexing of key phrases that indicate sentiment, like positive and negative comments on social media.
   * Document summarization and article generation for a given topic.

## Convolution Neural Network (CNN)   
CNN is type of Neural network that is designed to process input data that has grid-like structure such as image. It is commonly used in **computer vision**.   
They have three main types of layers, which are:-    
   * Convolutional layer
   * Pooling layer
   * Fully-connected (FC) layer

**Convolutional Layer** applies filters to the input image to extract features such as edges, textures, and shapes.   
The output of Convolutional layer is then passed to Pooling Layer.    

**Pooling Layer** is used to down-sample the image to reduce the spatial dimensions (computations) while retaining the most important information.   

**Fully Connected Layer** is used to make a prediction or classify the image.   

![example](https://github.com/Sazad123/SazRep/assets/119056368/e96bb891-d759-4b02-8129-89292b168dd6)

CNNs are trained using a large dataset of labeled images, where the network learns to recognize patterns and features that are associated with specific objects or classes. Once trained, a CNN can be used to classify new images, or extract features for use in other applications such as object detection or image segmentation.   
# Getting Started with R-CNN, Fast R-CNN, and Faster R-CNN    
Object detection is the process of finding and classifying objects in an image. One deep learning approach, regions with convolutional neural networks (R-CNN), combines rectangular region proposals with convolutional neural network features.  
R-CNN is a two-stage detection algorithm. The first stage identifies a subset of regions in an image that might contain an object. The second stage classifies the object in each region.  

## Object Detection Using R-CNN Algorithms  
Models for object detection using regions with CNNs are based on the following three processes:  
   * Find regions in the image that might contain an object. These regions are called region proposals.  
   * Extract CNN features from the region proposals.
   * Classify the objects using the extracted features.

There are three variants of an R-CNN. Each variant attempts to optimize, speed up, or enhance the results of one or more of these processes.   
**1) R-CNN**   
The R-CNN detector first generates region proposals using an algorithm such as Edge Boxes. The proposal regions are cropped out of the image and resized. Then, the CNN classifies the cropped and resized regions. Finally, the region proposal bounding boxes are refined by a support vector machine (SVM) that is trained using CNN features.  

**2) Fast R-CNN**  
Fast R-CNN uses an algorithm like Edge Boxes to generate region proposals. Unlike the R-CNN detector, which crops and resizes region proposals, the Fast R-CNN detector processes the entire image. Whereas an R-CNN detector must classify each region, Fast R-CNN pools CNN features corresponding to each region proposal. Fast R-CNN is more efficient than R-CNN, because in the Fast R-CNN detector, the computations for overlapping regions are shared.  

**3) Faster R-CNN**  
The Faster R-CNN detector adds a region proposal network (RPN) to generate region proposals directly in the network instead of using an external algorithm like Edge Boxes. The RPN uses Anchor Boxes for Object Detection. Generating region proposals in the network is faster and better tuned to your data. 
![RCNN_eg](https://github.com/Sazad123/SazRep/assets/119056368/d4c26cff-dc1f-4d42-af47-758cbe0b3056)

**--------------------------------------------------------------------------------------------------------------------------------------------------------------**

