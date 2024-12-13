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
- **TensorFlow**: For building the image recognition model.  
- **Kaggle**: Dataset sourcing and preprocessing.  
- **Keras**: High-level API for efficient ML model development.  
- **Python**: For scripting, model training, and integration.

### Cloud Computing
- **Postman**: API testing and development.  
- **Google Cloud Platform (GCP)**: Hosting and deploying the ML model and app backend.  
- **Flask, Express**: Backend development for API integration.  
- **PostgreSQL**: Database management for user.

### Mobile Development
- **Android Studio**: Development enviroment for building the app.
- **Kotlin**: Programming language for app development.
- **Dependencies/libraries**: Room, Retrofit, Datastore, Glide.
- **Design**: Figma.


## Documentation
### Machine learning
#### Plant Disease Detection
This model is designed to identify plant diseases from images using transfer learning technique. By analyzing patterns, textures, and visual symptoms in plant images, the model provides accurate diagnoses of 38 possible classification. 

#### model details
Architecture: using MobilenetV3Large as our base model and adding our own Dense layers for efficent image classification  
Dataset: Trained on a large image dataset of 38 different plant diseases found in kaggle
   
### Cloud Computing
#### Backend
The backend for the Plant Disease Detection application was developed using the Flask framework and for authentication using Express.js. 
#### Deployment
The backend, including pre-trained machine learning models, is deployed in Google Cloud Run. Cloud Run allows the backend to scale automatically based on incoming requests, ensuring efficient use of resources and handling varying levels of traffic. 
#### API Endpoints
The backend exposes secure API endpoints for mobile applications to interact with the cloud services. These endpoints include:
**1. User Authentication and Authorization**
- POST /users for registration
- POST /login for login user
- GET /profile for view the profile
- DELETE /logout for exit the app
**2. Image Upload and Disease Detection**
- POST /predict/upload: Used for detecting plant diseases from an image file that is either captured or uploaded from the gallery.
- POST /predict/base64: Used for detecting plant diseases from a live scan image, sent as a Base64-encoded string.

### Mobile Development
This application was developed with the MVVM (Model-View-ViewModel) architecture which aims to ensure application development runs in a modular, structured manner and makes further development easier. 
This application has several features that are directly connected to the API, such as login, sign up and photo scanning features for results. We also use Room Database as local storage to store data from history

## Further Development
1. chatbot implementation: users will be able to consult about their plant disease problem in our app
2. designated courses: partnership with farmers will allow us to create our own courses which will include videos about plant diseases that we created


## Group Members
| Name                          | Bangkit ID     | Learning Path       |
|-------------------------------|----------------|---------------------|
| Muhammad Arfian Praniza       | M229B4KY2737   | Machine Learning    |
| Muhammad Faizal Pratama       | M753B4KY2814   | Machine Learning    |
| Muhammad Zharfan              | M476B4KY3134   | Machine Learning    |
| Alzena Cikal Bhagaskara       | C249B4KY0444   | Cloud Computing     |
| Radinda Putri Salsabila       | C249B4KX3568   | Cloud Computing     |
| Bagus Abdul Wahhab            | A622B4KY0791   | Mobile Development  |
| Banu Eka Prayoga              | A622B4KY0811   | Mobile Development  |
