# Raspberry-Pi-Obstacle-Detection
Detecting obstacles using a PIR sensor and Raspberry Pi camera module. When the PIR sensor detects any motion, an image is captured and then processed using image analysis, filtering, and segmentation techniques.
# Requirements
a) Raspberry Pi 3 Model B+

b) Pi Camera

c) PIR Sensor

d) Jumper Wires

e) OpenCV
# Raspberry Pi Model 3B+
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/4744f813-0b6b-466a-9a23-b827d45a4668)

# Raspberry Pi OS/Raspbian
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/00221414-6b60-4898-85f9-d42fa97bc66c)

# Raspberry Pi Camera
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/c9b4f8b9-d9bb-4cb1-b5f4-eb86b64b6f45)
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/f78ef6b0-3fab-433d-b231-212f67535fe0)

# PIR Sensor
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/19ead74f-5b2f-42e7-bd68-943d710af342)


# OpenCV
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/edf82a48-4abc-49a8-88b0-e8b62e71f82b)

# Block Diagram
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/8b3095d6-16cd-441c-84cf-807ce47c16ec)

# Flowchart
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/59e30696-42dd-49dd-a858-7230c494e790)

# Circuit Diagram
Connect the Vcc pin of PIR Sensor to Pin 2 of Raspberry Pi, Gnd pin of PIR Sensor to pin 6 of Raspberry Pi and the Out pin of PIR Sensor to Pin 18 of the Raspberry Pi. 

Connect the Pi Camera to the slot provided on the Raspberry Pi.

![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/8e3c4b92-ba54-4a07-a1dd-33d2e46f8d7e)

# Code Explanation
1) This is a Python code for obstacle detection using a Raspberry Pi, a PIR (Passive Infrared) sensor and a camera. The code captures an image when motion is detected by the PIR sensor, performs image analysis, filtering and segmentation on the captured image, and displays the processed image on the screen.

2) The code starts by importing the necessary libraries, including RPi.GPIO for controlling the PIR sensor and OpenCV (cv2) for image processing. It then sets up the PIR sensor and the camera using their respective pins.

3) The code enters a loop that continuously checks the state of the PIR sensor. When motion is detected, it waits for a short period of time and then captures an image using the camera.

4) The captured image is then processed using various image processing techniques such as converting the image to grayscale, performing edge detection using the Canny algorithm, and filtering the image using a Gaussian filter. Finally, the image is segmented using thresholding and contours are drawn around the detected objects.

5) The processed image is displayed on the screen using the OpenCV imshow function. The user is prompted to press a key to close the window and the processed image is saved to a file. The loop continues to wait for motion to be detected by the PIR sensor, and the process repeats.

6) Finally, the code cleans up by releasing the camera and cleaning up the GPIO pins.

# Setup
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/40f3e684-ac72-4c74-8b43-15b4e6134127)
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/247794a2-ffd2-4634-8336-678436242a61)

# Results
The processed, filtered and edge detected images of a water bottle and computer monitor
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/cc243965-5284-4df0-9c34-6c8083c4a679)


The processed, filtered and edge detected images of two members of the project group
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/026b9959-fc8d-4864-aff5-5cdab4a372e1)


The processed, filtered and edge detected images of two friends
![image](https://github.com/KarthikT23/Raspberry-Pi-Obstacle-Detection/assets/119528503/4cbf39ce-f5a0-4bb3-a2e5-90b78c6918ad)

# References
[1] Li, Z., Li, B., Li, S., Li, Y., & Zhang, C. (2020). Real-time moving obstacle detection and tracking based on Raspberry Pi. In 2020 IEEE International Conference on Information and Automation (ICIA) (pp. 1174-1179). IEEE.

[2] Patel, D., & Patel, N. (2019). Real-time object detection and tracking using Raspberry Pi. In 2019 International Conference on Automation, Computational and Technology Management (ICACTM) (pp. 1-5). IEEE.

[3] Wang, H., Wu, L., & Gao, L. (2017). Obstacle detection for visually impaired people based on stereo vision and Raspberry Pi. In 2017 2nd International Conference on Image, Vision and Computing (ICIVC) (pp. 461-465). IEEE.

[4] Singh, P. K., Kumar, A., & Kumar, A. (2020). Real time obstacle detection and avoidance using Raspberry Pi. In 2020 International Conference on Power Electronics, Smart Grid and Renewable Energy (PESGRE) (pp. 358-362). IEEE.

[5] Dhivya, S., Gokulakrishnan, S., & Sivakumar, P. (2019). Raspberry Pi based obstacle detection and avoidance system for visually impaired people. In 2019 International Conference on Vision Towards Emerging Trends in Communication and Networking (ViTECoN) (pp. 1-5). IEEE.

[6] https://www.hackster.io/mjrobot/real-time-obstacle-avoidance-with-raspberry-pi-eb5a4a

[7] https://www.instructables.com/Obstacle-Detection-Using-Raspberry-Pi/

[8] https://circuitdigest.com/microcontroller-projects/raspberry-pi-obstacle-avoidance-robot-using-ultrasonic-sensors

[9] https://towardsdatascience.com/how-to-detect-obstacles-in-a-room-with-a-raspberry-pi-785e50c51e9b

[10] https://github.com/Ewenwan/RaspberryPi_ObstacleDetection
