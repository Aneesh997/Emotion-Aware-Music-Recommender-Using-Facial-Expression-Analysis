# MoodSync – Real-Time Emotion Based Music Recommendation System

## Overview

**MoodSync** is an AI-powered music recommendation web application that detects a user's facial emotion in real time and recommends mood-based music playlists using **Spotify integration**. The project combines Deep Learning, Computer Vision, Affective Computing, and Music Recommendation techniques to create a personalized and interactive music listening experience.

The system uses a **CNN-VGG19** based facial emotion recognition model trained on the **FER-2013 dataset** to classify emotions such as happy, sad, angry, neutral, surprise, disgust, and fear using live webcam input. Based on the detected emotion, the application automatically fetches and plays suitable playlists using the **Spotify Web API**.

The application was developed using **Flask** for the backend, **OpenCV** for face detection and image preprocessing, **TensorFlow/Keras** for deep learning model implementation, and **HTML/CSS/JavaScript** for the frontend interface.

---

## Features

- Real-time facial emotion detection
- CNN-VGG19 based emotion classification
- Spotify API integration for music recommendation
- Live webcam-based mood analysis
- Real-time playlist generation and playback
- Flask-based web application
- Interactive frontend UI
- OAuth 2.0 Spotify authentication
- Mood-based personalized recommendations
- Low latency real-time processing

---

## Technologies Used

### Frontend
- HTML
- CSS
- JavaScript
- AJAX

### Backend
- Flask
- Python

### AI / Machine Learning
- TensorFlow
- Keras
- OpenCV
- CNN (Convolutional Neural Network)
- VGG19

### APIs and Services
- Spotify Web API
- OAuth 2.0 Authentication

---

## Project Workflow

1. Webcam captures the user's face in real time
2. OpenCV detects and preprocesses the face image
3. CNN-VGG19 model predicts the user emotion
4. Detected mood is mapped to a Spotify playlist
5. Spotify API fetches and plays songs automatically
6. Frontend displays mood analysis and playback controls

---

## Project Structure

    project/
    │
    ├── static/
    ├── templates/
    ├── model/
    ├── dataset/
    ├── app.py
    ├── requirements.txt
    ├── README.md
    └── emotion_model.h5

---

## FER-2013 Dataset

The project uses the **FER-2013** facial emotion recognition dataset for training the CNN model.

**Dataset Link:** https://www.kaggle.com/datasets/msambare/fer2013

Download the dataset and place it inside the project `dataset` folder.

---

## Pretrained Model

The pretrained CNN-VGG19 model (`emotion_model.h5`) should be placed inside the project directory before running the application.

You can either:

- Train the model using the FER-2013 dataset
- Or use your already trained pretrained model file

---

## Installation

### Clone the Repository

    git clone <your-github-repository-link>
    cd MoodSync

### Install Dependencies

    pip install -r requirements.txt

---

## Run the Project

    python app.py

If your system uses Python 3 explicitly:

    python3 app.py

The application will start locally at: `http://127.0.0.1:5000`

---

## Required Setup

Before running the project:

1. Install all dependencies from `requirements.txt`
2. Download the FER-2013 dataset
3. Add your pretrained model file (`emotion_model.h5`)
4. Configure Spotify API credentials
5. Enable an active Spotify device for playback

---

## Performance

| Metric                              | Value     |
|-------------------------------------|-----------|
| Real-time emotion detection latency | ~150ms    |
| Emotion detection accuracy          | ~93%      |
| Webcam processing                   | Real-time |
| Playlist recommendations            | Dynamic   |

---

## Advantages

- Personalized music recommendations
- Real-time AI-based emotion analysis
- Interactive and user-friendly interface
- Seamless Spotify integration
- Low latency processing
- Emotion-aware intelligent system

---

## Future Improvements

- Multi-user support
- Better emotion classification
- Offline playlist caching
- Multi-modal emotion analysis
- Mood history tracking
- Additional music platform integration
- Advanced recommendation engine

---

## Learning Outcomes

Through this project, the following skills were developed:

- Deep Learning using CNN and VGG19
- Facial Emotion Recognition using OpenCV
- Spotify API Integration and OAuth Authentication
- Real-Time Computer Vision System Development
- Full Stack Web Development using Flask and JavaScript

---

## Authors

- Aneesh Adithya SR
- Shreyas Ghanathe
- Gauravi Suryavamshi
- Gopika R

---

## License

This project is developed for academic and educational purposes.
