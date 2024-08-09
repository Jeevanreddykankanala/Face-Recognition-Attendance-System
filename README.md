Face Recognition-Based Attendance System

Overview :
This project is a real-time face recognition-based attendance system that uses computer vision and facial recognition technologies to track attendance. The system captures video from a webcam, detects faces, recognizes them against a pre-loaded dataset of known faces, and logs attendance in an Excel file. It also includes blink detection to ensure that the person is present and attentive.

Features :
Face Recognition: Matches faces in real-time with known faces stored in the system.
Blink Detection: Monitors eye movements to confirm attention and presence.
Attendance Logging: Records attendance with date and time in an Excel file.
Dynamic Excel File Creation: Creates a new Excel file for each session with a timestamp for uniqueness.
Real-time Video Processing: Processes video frames in real-time for face recognition and blink detection.

Requirements :
Python 3.x
OpenCV
dlib
face_recognition
openpyxl
scipy

Configuration : 
Known Faces Directory
Place images of known faces in the known_faces directory. Ensure that the filenames follow the format name_registernumber.jpg/png.
Update Paths
Update the paths in the script to point to the correct locations of the known faces directory and the shape predictor file if needed.

How It Works : 
Initialization: The script initializes the Excel workbook for logging attendance if it doesn't already exist.
Face Recognition: It loads known faces and their encodings from the known_faces directory.
Video Capture: It starts capturing video from the webcam.
Face Detection: Faces are detected and compared with known faces in real-time.
Blink Detection: The system calculates the Eye Aspect Ratio (EAR) to detect blinks.
Logging: When a recognized face blinks, attendance is logged with date and time.
Display: The status (e.g., "Present" or "Face not Clear") is displayed on the video feed.

Limitations :
Performance may vary with lighting conditions and camera quality.
Accuracy may be affected by facial changes or accessories like glasses and masks.
Large datasets may require optimization for efficient processing.

Future Enhancements :
Integrate multi-factor authentication (e.g., voice or fingerprint recognition).
Improve handling of low-light and outdoor conditions.
Implement additional security and privacy measures.

Contact :
For any questions or feedback, please contact jeevanreddykankanala4321@gmail.com

