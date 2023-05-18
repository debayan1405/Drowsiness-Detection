# Drowsiness Detection Model Version 1:
This project utilized the following datasets:
<br>
* Driver Drowsiness Dataset (DDD): https://www.kaggle.com/datasets/ismailnasri20/driver-drowsiness-dataset-ddd
* Yawn Dataset: https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new

<br><br>
Data Augmentation was performed on these datasets by namely flipping the images, altering brightness/contrast and also applying blurring. As a result, we were able to increase the size of our dataset by 6 times to almost 340k images. The code for data augmentation can be found withing `data_augmentation.ipynb` file
<br><br>
Followed by this a Convolutional Neural Network was trained for 20 epochs, with 0.02 validation split and a batch size of 32. Also, the optimizer used is Adam with the sparse categorical cross-entropy loss function. You will find the details of the model structure in the `CNN_model.ipynb` file
<br><br>
The model was able to achieve an **accuracy of 90.009%** in the validation phase and therefore, we further interfaced it with the webcam in order to make use to it in real-time scenarios. The implementation code for this is available within `webcame_testing.ipynb` file
<br><br>
We also made use of the Frontal Face HAAR Cascade pre-trained model by OpenCV in order to extract just the face from the entire image and feed it into the model, thereby making our model independent of the distance of the face from the camera as well as in situations where no face can be detected 
<br><br>
At present we are processing around 1 Frame per second due to hardware constraints
<br><br>
In the future, the aim is to further extend this project and make the detection system more robust by testing out different models like R-CNNs and Transformers as well as improving the structure of the current model
