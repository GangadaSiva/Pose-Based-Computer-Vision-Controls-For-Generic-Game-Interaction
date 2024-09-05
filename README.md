Pose-Based Computer Vision Controls for Generic Game Interaction
This project introduces an innovative game controller that leverages computer vision techniques to enable hands-free interaction with games, specifically targeting the popular game Subway Surfers. Using Mediapipe for real-time pose detection, this system allows players to control in-game movements through body gestures like jumping, crouching, and side-stepping.

Features
Pose Detection: Implements Mediapipe's Pose solution to detect and track key body landmarks in real-time.
Hands-Free Game Control: No need for physical controllers—players control the game using body movements.
Real-Time Interaction: Smooth and responsive game control, with no noticeable delays, ensuring a seamless gaming experience.
Gesture-Based Commands: Map gestures like jumping, crouching, and side-stepping to corresponding in-game actions.
Automated Game Start: The game starts when the user’s hands are joined.
Python and OpenCV Integration: Uses OpenCV for video capture and Pyautogui for simulating keyboard inputs.
Customizable and Scalable: Adaptable to other games or applications by modifying the gesture mappings and controls.
Technologies Used
Python
Mediapipe: For pose detection
OpenCV: For video capture and image processing
Pyautogui: For simulating keyboard inputs based on detected gestures
Prerequisites
Before running the project, ensure you have the following installed:

Python 3.x
OpenCV (pip install opencv-python)
Mediapipe (pip install mediapipe)
Pyautogui (pip install pyautogui)
Installation
Clone this repository: git clone https://github.com/your-repo/game-pose-controls.git
Navigate to the project directory: cd game-pose-controls
Install the required dependencies: pip install -r requirements.txt
How It Works
Video Capture: The system captures live video input using the user's webcam.
Pose Detection: Using Mediapipe, the system detects body landmarks in real-time to interpret gestures.
Gesture Recognition: Gestures like jumping (raising hands), crouching (bending down), and side-stepping (leaning left/right) are recognized.
Game Control: Based on the recognized gestures, the system simulates key presses (e.g., spacebar for jump, arrow keys for movement) to control the in-game character.
Running the Project
Ensure your webcam is connected and functioning.
Run the main Python script: python main.py
Once the program starts, the webcam feed will be displayed. The system will detect your body movements and map them to corresponding game controls in Subway Surfers.
The game starts automatically when your hands are joined.
Customization
To modify gesture mappings or game controls, you can edit the gesture_control.py file. Adjust the conditions for detecting gestures and assign different key presses based on your needs.
Limitations
Requires adequate lighting conditions for accurate pose detection.
The system is currently tailored for Subway Surfers, but can be adapted to other games by modifying key bindings.
Future Enhancements
Expand support to more games by adding custom gesture mappings.
Improve gesture recognition accuracy in diverse environments.
Add a calibration feature to adapt to different users' body types.
Contributing
Feel free to fork this repository and contribute to the project. Pull requests are welcome!


Acknowledgements
Mediapipe by Google for their Pose solution.
OpenCV and Pyautogui libraries for video capture and input simulation.
