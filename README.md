# Hand Gesture Controlled Steering

This project enables gesture-based control using hand tracking, allowing directional control based on hand movements. Built using Python, OpenCV, and MediaPipe, the system interprets specific hand gestures to simulate key presses for directional navigation.

## Features

- Detects hand gestures and positions via webcam input.
- Commands simulated key presses to control movement:
  - **W**: Move forward
  - **A**: Turn left
  - **S**: Move backward
  - **D**: Turn right
- Dynamic hand tracking with visual feedback displayed on the screen.

## File Overview

### `steering.py`
Contains the main logic for gesture-based steering control:
- Captures hand landmarks with MediaPipe.
- Calculates positions and interprets gestures for directional control.
- Displays feedback on the screen using OpenCV.

### `keyinput.py`
Handles keyboard input using ctypes:
- Maps keys for movement (`W`, `A`, `S`, `D`).
- Contains functions to simulate key presses and releases based on detected gestures.

## Requirements

- Python 3.x
- OpenCV (`cv2`)
- MediaPipe (`mediapipe`)
- ctypes (included with Python)

Install dependencies using:

```bash
pip install opencv-python mediapipe
