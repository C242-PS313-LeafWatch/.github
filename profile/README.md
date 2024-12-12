# LeafWatch
welcome to LeafWatch!, Plant diseases can cause significant losses for farmers, particularly in Indonesia, where small-scale farmers often lack access to affordable diagnostic tools and practical knowledge. This project aims to empower farmers with a mobile application that leverages machine learning to detect plant diseases, provide treatment insights, and offer educational resources to ensure better crop management and reduce losses.

## Overview
This mobile app is designed to address the challenges of plant disease identification by using cutting-edge machine learning algorithms. With its user-friendly interface, farmers can easily take photos of plants and instantly receive a diagnosis. The app also offers a detection history log, educational videos, and a library of general information about plant diseases to support continuous learning.

## Features
Plant Disease Detection: Upload plant images to identify diseases using ML-based image recognition.  
User-Friendly Interface: An intuitive design that makes the app accessible for all users, including farmers with minimal tech experience.  
Detection History: A log of previous scans for users to track patterns and manage their crops better.  
Educational Videos: Curated content to help farmers learn about plant disease prevention, treatment, and best practices.  
General Information on Plant Diseases: A library of resources covering common plant diseases, symptoms, and remedies.

## Technology Stack
### Machine Learning
TensorFlow: For building the image recognition model.  
Kaggle: Dataset sourcing and preprocessing.  
Keras: High-level API for efficient ML model development.  
Python: For scripting, model training, and integration.

### Cloud Computing
Postman: API testing and development.  
Google Cloud Platform (GCP): Hosting and deploying the ML model and app backend.  
Flask: Backend development for API integration.  
PostgreSQL: Database management for user and detection history.

### Mobile Development
Android Studio: Development environment for building the app.  
Kotlin: Programming language for app development.


## Documentation
### Machine learning
#### Plant Disease Detection
This model is designed to identify plant diseases from images using transfer learning technique. By analyzing patterns, textures, and visual symptoms in plant images, the model provides accurate diagnoses of 38 possible classification. 

#### model details
Architecture: using MobilenetV3Large as our base model and adding our own Dense layers for efficent image classification  
Dataset: Trained on a large image dataset of 38 different plant diseases found in kaggle
   
### Cloud Computing
### Mobile Development
This application has the main feature of sending files in the form of images to a model stored in the cloud and displays the results of the analysis and recommendations for treatment videos from YouTube. Dependencies used are Retrofit, Gson, Room, LiveData, and LiveModel


## Further Development
1. chatbot implementation: users will be able to consult about their plant disease problem in our app
2. designated courses: partnership with farmers will allow us to create our own courses which will include videos about plant diseases that we created


## Group Members
1. Muhammad Zharfan
2. Muhammad Arfian Praniza 
3. Muhammad Faizal Pratama 
4. Alzena Cikal Bhagaskara 
5. Radinda Putri Salsabila 
6. Bagus Abdul Wahhab
7. Banu Eka Prayoga 
