# OpenPose-based-posture-detection
OpenPose is a real-time multi-person system to detect human body keypoints (like joints) from images or video. It gives precise coordinates of body parts like the neck, shoulders, hips, knees, elbows, etc.

# You're using OpenPose to analyze a webcam image and then:
1. Extract body keypoints (e.g., positions of neck, hips, knees, etc.).
2. Calculate angles or distances between these keypoints.
3. Classify the person's sitting posture based on the body shape formed.

# Tools Used:
1. OpenCV: Captures webcam frame
2. OpenPose Wrapper: Extracts keypoints from the frame
3. Your Custom Logic: Uses geometry (angles & distances) to label posture

## 2. Posture Detection Using Ultrasonic Sensors
Input: Distance data from an Arduino via serial port
Sensors:
1.Back Sensor (behind the chair): Measures how far the back is from the backrest
2. Side Sensor (side of the chair): Measures lean from side
Process:
If the distance is too short or too long, it assumes bad posture:
Slouching
Reclining
Output: A separate label indicating posture

