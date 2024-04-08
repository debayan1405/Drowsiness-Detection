# Application of Convolutional Neural Networks in Drowsiness Detection using Facial Features:

1. Obtained a comprehensive dataset comprising over 340,000 images through a combination of the Driver Drowsiness Dataset (DDD) and Yawn Dataset, augmented sixfold using advanced techniques. This extensive dataset served as the cornerstone for robust model training and validation.

2. Implemented the HAAR Cascade Frontal face detector to accurately identify and extract tightly cropped images around the face, ensuring focus solely on relevant facial features.

3. Developed a tailored Convolutional Neural Network (CNN) architecture for drowsiness detection, undergoing rigorous training over 20 epochs with meticulous parameter tuning. Utilizing the Adam optimizer and sparse categorical cross-entropy loss function, the model achieved an impressive validation accuracy of 90.13%.

4. Engineered a testing interface leveraging OpenCV, seamlessly integrating with live video feeds for real-time analysis. With the capability to process frames at a rate of 1 fps (on CPU), the interface accurately computed the drowsiness percentage, providing timely insights into the driver's alertness level.

5. Implemented a frame counter mechanism within the testing interface to mitigate false positives and account for temporal dynamics, enhancing the system's reliability in real-world scenarios.

6. Ongoing development focuses on exploring alternative model architectures and optimization strategies, with a specific emphasis on developing lightweight implementations suitable for deployment on embedded systems within vehicles. This extension aims to broaden the solution's applicability and scalability across diverse operational environments.
