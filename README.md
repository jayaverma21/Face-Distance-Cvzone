# Face-Distance-Cvzone
# Face Distance Measurement using OpenCV

This project demonstrates an application that detects faces from a webcam feed, calculates the approximate distance from the camera to the detected face, and displays the distance on the screen using OpenCV.

## Requirements

- Python 3.x
- OpenCV

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/yourusername/face-distance-measurement.git
    cd face-distance-measurement
    ```

2. Make sure you have the Haar Cascade classifier file (`myhaarcascade_frontalface_default.xml`) in the project directory.

3. Install the required packages:

    ```bash
    pip install opencv-python
    ```

## Usage

1. Run the script:

    ```bash
    python face_distance_measurement.py
    ```

2. The webcam feed will open in a new window. The script will detect faces, draw rectangles around them, and display the approximate distance from the camera to each detected face in centimeters.

3. Press the 'Enter' key to exit the application.

## Code Overview

The main script performs the following steps:

1. Initializes the Haar cascade classifier for face detection.
2. Opens a webcam feed and reads frames in a loop.
3. Converts each frame to grayscale and detects faces using the Haar cascade classifier.
4. For each detected face, calculates the approximate distance from the camera using a known face width and the focal length of the camera.
5. Draws a rectangle around each detected face and displays the calculated distance above the rectangle.
6. Displays the annotated frame with face rectangles and distance measurements.
