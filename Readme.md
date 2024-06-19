# Gesture Controlled Mouse

## Overview

This project implements a gesture-controlled mouse using a camera to track hand movements. It leverages OpenCV for video capture, Mediapipe for hand tracking and gesture recognition, PyAutoGUI for mouse and keyboard control, PyCaw for audio control, and Screen Brightness Control for adjusting the screen brightness.

## Features

- **Mouse Movement**: Control the mouse cursor with hand movements.
- **Clicking**: Perform left, right, and double clicks using specific hand gestures.
- **Scrolling**: Scroll vertically and horizontally using pinch gestures.
- **Volume Control**: Adjust the system volume with pinch gestures.
- **Brightness Control**: Adjust the screen brightness with pinch gestures.

## Requirements

- Python 3.x
- OpenCV
- Mediapipe
- PyAutoGUI
- PyCaw
- Screen Brightness Control

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/manan18/Gesture-Control--ML-Project.git
    cd Gesture-Control--ML-Project
    ```

2. Install the required packages:
    ```sh
    pip install opencv-python mediapipe pyautogui pycaw screen-brightness-control
    ```

## Usage

1. Run the gesture controller:
    ```sh
    python gesture_control.py
    ```

2. The application will start capturing video from the default camera. Ensure your hand is visible in the camera frame.

3. Use the following gestures to control the mouse and system features:
    - **Move Cursor**: Move your hand to move the cursor.
    - **Left Click**: Make a fist gesture.
    - **Right Click**: Point with your index finger.
    - **Double Click**: Make a two-finger closed gesture.
    - **Scroll**: Use a pinch gesture with your minor hand (non-dominant).
    - **Adjust Volume**: Use a pinch gesture with your major hand (dominant).
    - **Adjust Brightness**: Use a pinch gesture with your major hand (dominant).

## Code Structure

- `gesture_control.py`: Main script to start the gesture controller.
- `Gest`: Enum class for mapping all hand gestures to binary numbers.
- `HLabel`: Enum class for multi-handedness labels.
- `HandRecog`: Class for converting Mediapipe landmarks to recognizable gestures.
- `Controller`: Class for executing commands according to detected gestures.
- `GestureController`: Class for managing video capture and processing.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## Acknowledgements

- OpenCV
- Mediapipe
- PyAutoGUI
- PyCaw
- Screen Brightness Control

## Contact

For any inquiries or feedback, please contact [mananchawla12@gmail.com].
