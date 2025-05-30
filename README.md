# Campus Navigation App 🏫📍

An AI-powered mobile application that helps users navigate campus landmarks using computer vision and machine learning. The app can identify campus buildings from photos, estimate distances, and provide real-time navigation assistance.

## 🎯 Project Overview

This project combines computer vision, machine learning, and mobile development to create an intelligent campus navigation system. Users can simply take a photo of a campus landmark, and the app will:

- **Identify the building** using deep learning classification
- **Estimate distance** to the landmark using depth estimation
- **Provide navigation** with real-time mapping and directions
- **Display results** with an intuitive mobile interface

## 🚀 Features

### 🤖 AI-Powered Recognition
- **Landmark Classification**: ResNet-based model trained on 282 campus images across 18 different buildings
- **Object Segmentation**: SAM (Segment Anything Model) for precise landmark detection
- **Distance Estimation**: ZoeDepth monocular depth estimation for accurate distance measurement

### 📱 Mobile Application
- **Cross-Platform**: Built with React Native and Expo for iOS and Android compatibility
- **Real-Time Processing**: Instant image analysis and prediction display
- **Interactive Maps**: Visual navigation with user location, landmark markers, and route visualization
- **Smooth Animations**: Enhanced user experience with fluid interface transitions

### 🔧 Backend Infrastructure
- **Flask API**: RESTful backend service for ML model integration
- **Docker Containerization**: Scalable deployment with containerized Flask application
- **Real-Time Processing**: Efficient image processing pipeline with multiple ML models

## 🏗️ Architecture

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Mobile App    │    │   Flask API     │    │   ML Models     │
│  (React Native) │◄──►│   (Backend)     │◄──►│   (PyTorch)     │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         │                       │                       ├── ResNet
         │                       │                       ├── SAM
         │                       │                       └── ZoeDepth
         │                       │
         └───────────────────────┼───────────────────────┘
                                 │
                        ┌─────────────────┐
                        │   Image Dataset │
                        │   (282 images)  │
                        └─────────────────┘
```

## 📊 Dataset

### Campus Landmarks Dataset
- **Total Images**: 282 high-resolution images
- **Buildings Covered**: 18 different campus landmarks
- **Image Quality**: 12MP+ resolution with varied lighting conditions and angles
- **Organization**: Structured folders with consistent naming conventions

### Covered Landmarks
- Admin Block
- Library
- Civil Engineering Building
- Fountain Garden
- Juice Shop
- Tennis Court
- Campus Gates
- Garden Areas
- Parking Areas
- And 9 more campus locations

## 🛠️ Technology Stack

### Frontend
- **React Native** - Cross-platform mobile development
- **Expo** - Development platform and tools
- **React Navigation** - Navigation library
- **Maps Integration** - Real-time location and mapping

### Backend
- **Flask** - Python web framework
- **PyTorch** - Deep learning framework
- **OpenCV** - Computer vision library
- **NumPy** - Numerical computing
- **Docker** - Containerization

### Machine Learning Models
- **ResNet** - Building classification
- **SAM (Segment Anything Model)** - Object segmentation
- **ZoeDepth** - Monocular depth estimation

## 🔄 Workflow

1. **Image Capture**: User takes a photo of a campus landmark
2. **API Request**: Mobile app sends image to Flask backend
3. **ML Processing**: 
   - ResNet classifies the building
   - SAM segments the landmark
   - ZoeDepth estimates distance
4. **Location Calculation**: User location estimated using landmark GPS and distance vector
5. **Response**: Backend returns annotated image, building name, confidence score, and distance
6. **Navigation**: App displays results and provides map-based navigation

## 📱 Demo

Check out the `demo.mp4` file to see the app in action!

## 🎯 Key Achievements

- **High Accuracy**: Robust landmark recognition across diverse lighting and weather conditions
- **Real-Time Performance**: Fast image processing and prediction delivery
- **User-Friendly Interface**: Intuitive mobile app with smooth animations
- **Scalable Architecture**: Containerized backend for easy deployment and scaling
- **Comprehensive Dataset**: Well-organized image dataset with proper annotations

## 🔮 Future Enhancements

- **Expanded Dataset**: Include more campus buildings and outdoor landmarks
- **Offline Mode**: Local model inference for areas with poor connectivity
- **AR Integration**: Augmented reality overlay for enhanced navigation
- **Multi-Language Support**: Internationalization for diverse user base
- **Voice Navigation**: Audio-guided directions and landmark descriptions

## 👥 Team Contributions

### Phase 1: Dataset Creation & Annotation
- Systematic image capture across 18 campus landmarks
- Quality control and consistent annotation methodology
- Organized dataset structure for ML training

### Phase 2: Machine Learning Development
- Model selection and training pipeline
- Distance estimation using stereo triangulation and monocular depth
- Performance optimization and accuracy validation

### Phase 3: Backend Development
- Flask API development and ML model integration
- Docker containerization and deployment setup
- API testing and validation with Postman

### Phase 4: Frontend Development & Integration
- React Native mobile app development
- Backend integration and error handling
- Map-based navigation and user interface design

## 📄 License

This project is developed for educational purposes as part of a campus navigation system initiative.

---

**Built with ❤️ for smarter campus navigation** 