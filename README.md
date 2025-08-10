# Real-time Biceps Curl Counter with AI-powered Pose Estimation

## Project Overview

This project implements a real-time gym curl counter that leverages computer vision and AI-powered pose estimation techniques to accurately detect, track, and count bicep curl repetitions. Using the **MediaPipe** library for pose detection and combining **LSTM** and **CNN** models, the system tracks key joint coordinates and calculates arm angles to count repetitions, offering real-time feedback to users during their workout.

## Key Features

- **Pose Estimation**: Uses MediaPipe for accurate joint detection (shoulder, elbow, wrist) to monitor arm movements.
- **Repetition Counting**: Counts bicep curls based on joint angles, using an LSTM and CNN-based model to identify successful repetitions.
- **Real-time Feedback**: Displays real-time repetition count and exercise progress through an intuitive graphical interface.
- **Adaptable to Lighting Conditions**: Works in varied lighting conditions and can handle different user poses.
- **Visualization**: Shows detected landmarks and joint connections for better understanding of pose estimation.

## Project Setup

### Prerequisites

- Python 3.x
- pip (Python package installer)
- ### Installation Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/bicep-curl-counter.git
   cd bicep-curl-counter
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3.The requirements.txt should include:

mediapipe
opencv-python
tensorflow
numpy
matplotlib

Run the application:
After setting up the dependencies, you can start the system with the following command: 
    ```bash 
 python bicep_curl_counter.py



This will initiate the webcam feed, start detecting your arm movements, and begin counting your repetitions.

## Usage
Step 1: Ensure your webcam is properly set up.

Step 2: The system will display the camera feed, overlaying detected keypoints (shoulders, elbows, wrists) to visualize your movement.

Step 3: Begin performing bicep curls. The system will automatically count the repetitions and display the real-time count on the interface.

Step 4: The system provides feedback about the current exercise stage, helping users stay motivated and track performance.

## Algorithm
Pose Detection:

The system uses MediaPipe to detect the keypoints (shoulder, elbow, wrist) of the user’s arm.

Angle Calculation:

Custom functions compute angles between these joints, helping to determine the position of the arm during the curl (e.g., fully extended, fully contracted).

Repetition Recognition:

Using an LSTM and CNN model, the system analyzes the movement sequence over time to count the repetitions accurately based on predefined angle thresholds.

Real-time Feedback:

The repetition count and current stage of the exercise (e.g., up or down) are displayed to the user during the workout.

## Results
The system was tested for accuracy, achieving an accuracy of 87%, a precision of 85%, and a recall of 92%, ensuring reliable repetition counting across various lighting conditions and user poses.

Statistical Metrics:
**Precision:** 0.85

**Recall:** 0.92

**F1-Score:** 0.88

**Accuracy:** 0.87

Sample Output

