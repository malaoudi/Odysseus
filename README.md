# Odysseus
Odysseus Software and Hardware – A low-cost fall detection activity classifying camera system that consists of software and apparatus 
# Goal: 
To design a low-cost and home-safe camera that connects the camera from the structure apparatus, Odysseus, to a computer and then we utilize a particle microcontroller to enable cloud-based servo motor commands and compute trajectories for the head of Odysseus to track someone in its sight to enable falling detection of anyone in the room. 
Overview: This project was developed with classmates and we used it for a hackathon competition at the university. Odysseus was built through flask Web Server deployed on Google Cloud Platform. The Camera Client runs locally Runs OpenPose [Deep Learned Human Pose estimation model] Runs our manually trained multi-class SVM from outputted pose keypoints. This classifies the pose from [‘Standing’, ‘Sitting’, ‘Fallen’, ‘Background’] PID Controller determines angle to track human in the frame, which is posted to the Web Server. Web Server communicates with the Particle Photon (IOT device) to rotate servo using Pulse Width Modulation (PWM) signal. I worked on the web server, camera client, front end, OpenPose integration & SVC Pose classifier
# Tools: 
used Flask, Google Cloud, , opencv, openpose particle, hardware, cocoa gcp, bootstrap sklearn
