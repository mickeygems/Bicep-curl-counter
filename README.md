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

### Installation Steps

### Installation Steps

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
