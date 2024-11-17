## Spot Finder
Spot Finder is an AI-powered parking space detection system designed to simplify and automate the process of finding available parking spots in real-time. Utilizing computer vision and machine learning, Spot Finder accurately identifies open parking spaces, providing users with a seamless parking experience.

![image](https://github.com/user-attachments/assets/89bde7a5-026c-48fe-84fe-85bbf10a6fb7)

## Key Features

- Real-Time Detection: Spot Finder uses advanced computer vision algorithms to analyze live video feeds from parking lots, detecting available parking spots instantly.
  
- Pre-Trained Models: Leveraging pre-trained machine learning models, the system ensures high accuracy in detecting both occupied and vacant parking spaces.

- High Accuracy with Computer Vision: Powered by OpenCV and custom-trained models, Spot Finder delivers exceptional accuracy in identifying vehicles and free spaces, even in complex environments.

- Scalable Solution: The system is highly scalable, allowing deployment across various parking facilities, from small lots to large multi-level garages, with minimal setup requirements.

- User-Friendly Interface: Spot Finder provides a clean and intuitive interface, enabling users to quickly find and reserve parking spaces.

- Customizable for Different Parking Lots: The system is highly adaptable, supporting various camera placements and parking configurations, making it suitable for any layout.

---

## How It Works

### Parking Spot Identification
The parking lot is divided into individual spots using `cv2.connectedComponentsWithStats`.

### Frame Processing
Each frame is analyzed to detect changes in parking spots.  
Differences between the current and previous frame are calculated using `calc_diff`.

### Classification
A pre-trained Support Vector Classifier (SVC) predicts whether a spot is empty or occupied based on resized spot images.

### Visualization
Bounding boxes are drawn over parking spots:  
- Green for empty spots.  
- Red for occupied spots.

---

## Results

Spot Finder provides real-time updates on parking spot availability, accurately identifying the status of each spot and summarizing the total available spots.

---

## Technologies Used

- OpenCV: For image processing and real-time detection.
- Python: Backend programming for handling video feeds and model predictions.
- Pre-trained Machine Learning Models: For accurate detection of vehicles and parking statuses.
- Flask: For a user-friendly web interface to display parking information.

---

## Future Enhancements

- AI-Driven Predictions: Implement predictive models to forecast parking availability based on historical data.
  
- Mobile App Integration: Develop a mobile app to allow users to easily find and reserve parking spots using Spot Finder.

- Multi-Camera Support: Enable the system to support multi-camera setups for larger parking areas, ensuring comprehensive coverage.

---

Spot Finder is a reliable, accurate, and scalable solution for modern parking challenges, simplifying parking management and improving user experience.
