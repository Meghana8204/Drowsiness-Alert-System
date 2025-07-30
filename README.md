# Drowsiness-Alert-System

Driver fatigue and drowsiness are leading causes of road accidents, especially during night travel. The aim of this project is to detect signs of drowsiness (such as prolonged eye closure) using a non-invasive camera and computer vision techniques, and to alert the user before an accident can occur.

Technologies and Tools Used
Programming Language: Python
Libraries: OpenCV, Dlib, Imutils, Scipy
Platform: VS code
Alert Module: buzzer or screen warning

 Hardware Requirements
 Webcam (Laptop/USB)

Working Principle
A live video feed is captured using the webcam.
Face is detected using Dlib’s frontal face detector.
Facial landmarks (68 points) are identified.
From these, eye landmarks are used to calculate EAR (Eye Aspect Ratio).
When EAR value drops below a set threshold (e.g., 0.25) for a certain number of consecutive frames (e.g., 30), drowsiness is detected.
The system triggers a buzzer or visual alert to wake up the driver.

EAR Formula

EAR= 
2×∣∣p1−p4∣∣
∣∣p2−p6∣∣+∣∣p3−p5∣∣
 
Where p1 to p6 are eye landmark points.

Low EAR → Eyes are closed

High EAR → Eyes are open

 Thresholds Used
EAR threshold: 0.25
Consecutive frames threshold: 30
If the EAR remains below 0.25 for 30 frames continuously, drowsiness is assumed.

 Features of the System
Real-time monitoring with webcam
No wearable devices needed
Alerts when eyes stay closed too long
Can run on any standard PC/laptop
Open-source and customizable

 Applications
Driver safety systems (cars, buses, trucks)
Security room monitoring
Office fatigue detection
Personal use for long working hours

 Advantages
Non-invasive
Low-cost solution
Can be deployed using open-source tools
Prevents fatigue-related accidents

 Limitations
Performance can reduce in poor lighting
Might give false alerts if user is blinking frequently
Webcam quality affects accuracy

 Future Enhancements
Add yawn detection using mouth landmarks
Store alert logs in cloud database
Use deep learning (CNN) for better accuracy
Mobile version using OpenCV mobile SDK
Combine with voice alert system or vehicle control

 Internship Details
 Year: 2024–25
 Company: Techciti Software Consulting Pvt Ltd
 College: Navkis College of Engineering, Hassan
 Team Size: 1
