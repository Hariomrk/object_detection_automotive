AI-Based Vehicle Following Detection System
Project Aim

Detect if a vehicle is following another vehicle continuously and generate an alert using AI, tracking, and optional IoT integration.

Project Overview

This project is a real-time vehicle following detection system. Using YOLOv8/YOLOv11 and BYTETracker, vehicles in traffic videos are detected and tracked over time. The system identifies if a vehicle is continuously following another and raises alerts when unsafe following (tailgating) occurs.

Weekly Progress
Week 1 – Vehicle Detection and Tracking

Implemented YOLOv8 for vehicle detection in traffic videos.

Integrated BYTETracker for continuous tracking of detected vehicles.

Assigned unique tracker IDs to vehicles to maintain identification across frames.

Verified detection and tracking results with annotated video output.

Week 2 – Tailgating Detection

Developed a tailgating detection module using bounding box positions and pixel distance.

Implemented detect_tailgating() function to identify vehicles following too closely.

Highlighted tailgating vehicles in red bounding boxes with labels.

Created a separate output video (vehicle-tailgating-result.mp4) to preserve previous results.

Environment & Setup

Platform: Google Colab (Python 3)

Libraries & Tools:

ultralytics<=8.3.40 (YOLOv8)

ByteTrack (vehicle tracking)

supervision (video handling and annotations)

OpenCV (video processing)

Input Video: vehicle-counting.mp4

Output Videos:

Week 1: vehicle-counting-result.mp4 (tracking only)

Week 2: vehicle-tailgating-result.mp4 (tracking + tailgating detection)

Next Steps

Integrate real-time alerts (sound or IoT notifications) for tailgating vehicles.

Implement real-world distance estimation using perspective transformation for more accurate tailgating detection.

Optimize detection and tracking pipeline for real-time performance
