

# Classroom Analytics and Learning Evaluation using Computer Vision

## Overview

In modern educational settings, the ability to assess student engagement and attention levels in real-time is crucial for educators to adapt their teaching strategies effectively. Traditional methods of evaluating student participation, such as verbal responses or written assignments, often provide limited insight into the dynamics of classroom interactions. To address this challenge, we present a comprehensive approach called **"Classroom Analytics and Learning Evaluation using Computer Vision"**, which leverages state-of-the-art computer vision techniques to analyze student behavior and engagement patterns in a classroom environment.

This project aims to help educators understand and respond to student engagement by integrating person detection, face recognition, emotion detection, body landmark tracking, and activity recognition. Our system provides a holistic view of student behavior, allowing educators to identify actively participating students as well as those who may be disengaged or distracted.

## Core Methodology

### Person Detection
We use the YOLOv8 model for person detection, which provides bounding boxes around individuals in the classroom.

### Re-identification and Tracking
Deep SORT is applied to assign unique IDs to each person, enabling us to track their movements and interactions over time.

### Face Recognition and Emotion Detection
A face detection model identifies and extracts facial features, which are subsequently analyzed using the EmoAffectNet model to determine the emotional state of each student and classify it into 7 labels: 'Neutral', 'Happiness', 'Sadness', 'Surprise', 'Fear', 'Disgust', 'Anger'.

### Body Landmark Tracking
We utilize the Mediapipe model to detect body landmarks, such as keypoints representing the head, shoulders, and hands. These landmarks are then fed into a custom-trained DNN classification model, which categorizes the body activity into distinct labels such as 'looking forward', 'raising hand', 'sleeping', 'turning around', 'reading', or 'writing'.

### Engagement Classification
By combining the facial expression and body activity labels, we assign each student a final label of either "focused", "confused", "distracted", or "disengaged", providing educators with a comprehensive assessment of student engagement levels.


![image](https://github.com/tanmay910/Classroom_analytics_and_learning_evaluation/assets/105966781/7586f86b-c9ff-4951-902e-507d4344fe2b)

## Demo
#### Output of posture Model



## Significance

The project enhances the learning experience for both students and educators. Real-time feedback on student engagement allows educators to tailor their teaching strategies. Data from the system can identify trends and patterns in student behavior, enabling data-driven decisions to improve classroom dynamics and student outcomes.

## Repository

You can access the project repository on GitHub: [Classroom Analytics and Learning Evaluation](https://github.com/tanmay910/Classroom_analytics_and_learning_evaluation)

---

Feel free to modify the content as needed to better fit your project's specifics or personal preferences.
