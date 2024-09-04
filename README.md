# Real-Time Pose Detection System
This project is a real-time computer vision application that detects and tracks human body poses using a webcam or a video file. It utilizes MediaPipe's Pose solution to identify and visualize key landmarks on the human body, making it suitable for applications like fitness tracking, gesture recognition, and augmented reality.

![image](https://github.com/user-attachments/assets/b2533c51-8476-4b2d-93d0-d623e2b51b7f)
![image](https://github.com/user-attachments/assets/a9d96ff6-6252-4eef-8c67-9bde31675c9f)


## 1. Real-Time Pose Detection with OpenCV
The application captures live video feed from a webcam (cv2.VideoCapture(0)) or can be adapted to work with video files.

It processes each video frame in real-time, making it suitable for interactive applications requiring immediate pose feedback.
## 2. Pose Detection with MediaPipe
The system uses MediaPipe’s Pose solution, which accurately detects key landmarks on the human body such as shoulders, elbows, knees, and more.

The poseDetector class is implemented to manage pose detection and tracking, allowing configuration of detection and tracking confidence levels.
## 3. Drawing and Visualizing Body Landmarks
Detected body landmarks are drawn on the image using MediaPipe’s drawing utilities, connecting key points to form a skeleton overlay on the person’s body.

Custom drawing specifications such as thickness and color can be adjusted for better visualization.
## 4. Extracting Landmark Positions
The application extracts the coordinates of each detected landmark relative to the image size. These positions are stored in a list and can be used for further analysis or integration with other applications.

Specific landmarks can be highlighted or used to trigger actions, such as the example of drawing a red circle on the right elbow (lmList[14]).
## 5. Frame Rate Display
The frames per second (FPS) are calculated and displayed on the screen to provide feedback on the performance of the real-time detection system.
## 6. Application Flow
Initialization: The system initializes the webcam and sets up the pose detector with specified parameters.

Pose Detection: Each video frame is processed to detect body landmarks.

Landmark Visualization: Detected landmarks are drawn on the image for clear visualization of the pose.

Position Extraction: Landmark positions are extracted for potential further analysis.

Performance Monitoring: The FPS value is displayed to monitor real-time performance.
## Use Case
This project is suitable for applications that require pose estimation, such as fitness apps, motion capture for animation, sports analytics, and interactive experiences. It can be used to track body movements and analyze poses in real time, offering valuable insights and data for a wide range of scenarios.

Note: I do not own the copyrights of this project.(youtube @murtazasworkshop) It is for learning purposes only.

