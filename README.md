# Drowsiness_Detection_System
The Driver Drowsiness Detection System is a real-time safety tool that uses computer vision to detect drowsiness and yawning in drivers. It monitors eye closure (EAR) and tracks yawns using facial landmarks from a webcam, providing audio alerts to prevent accidents. Built with Python, OpenCV, and Dlib, it enhances road safety.

## Features
- Real-time video processing using OpenCV.
- Detects closed eyes and yawning using:
  - Eye Aspect Ratio (EAR).
  - Lip distance.
- Provides audible alerts for drowsiness or excessive yawning.
- Adjustable thresholds for eye closure and yawning detection.

## Requirements
- Python 3.8 or above
- A webcam or video feed for real-time processing

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/drowsiness-detection.git
   cd drowsiness-detection
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Place the required Haar cascade and shape predictor files in the same directory:
   - `haarcascade_frontalface_default.xml`
   - `shape_predictor_68_face_landmarks.dat`
2. Run the script:
   ```bash
   python drowsiness_detection.py
   ```
3. Press `q` to exit the application.

## Files
- **drowsiness_detection.py**: Main script for the project.
- **haarcascade_frontalface_default.xml**: Haar cascade for face detection.
- **shape_predictor_68_face_landmarks.dat**: Dlib shape predictor for facial landmarks.
- **requirements.txt**: List of required Python libraries.

## Thresholds
You can modify the following thresholds in the script to suit your requirements:
- `EYE_AR_THRESH`: Threshold for eye aspect ratio to detect drowsiness.
- `EYE_AR_CONSEC_FRAMES`: Number of consecutive frames to trigger an alert.
- `YAWN_THRESH`: Threshold for yawning based on lip distance.
- `YAWN_COUNT_THRESHOLD`: Number of consecutive yawns to trigger an alert.

## Dependencies
The following Python libraries are required for this project:
- OpenCV
- dlib
- imutils
- scipy
- numpy
- pyttsx3

You can find the dependencies in the `requirements.txt` file for easy installation.

## Credits
- Haar cascade XML file: [OpenCV GitHub Repository](https://github.com/opencv/opencv)
- Shape predictor: [Dlib library](http://dlib.net/)

## License
This project is licensed under the MIT License. See the LICENSE file for details.
