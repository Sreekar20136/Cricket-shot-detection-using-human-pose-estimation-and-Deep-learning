1. The main objective of this project is to  create a robust model for cricket shot detection using human pose estimation 
2. The dataset used consists of four cricket shot types with 900 images for each shot type
      1. Pull
      2. Drives
      3. Legglance flick
      4. Sweep
3. Data preprocessing
   1. Removed noisy images
   2. Resizing all images to a specific size
4. Then the preprocessed images are used for Cricket shot detection
5. Used Mediapipe for human pose estimation
6. Used Pretrained Vgg16 for extracting image features
7. The pose of the cricket shot image will be detcted only if it is greater than certain threshold
8. Image features are considered for the images if and only if the pose features are extracted for thr image for detecting the cricket shot
9. The combined image features and pose features are then given to the custom deep learning model to detect the the cricket shots
10. The custom deep learning model created conists of dense layer with 256 units followed by a dropout  layer and dense layer again followed softmax layer for detecting the cricket shot
11. This hybrid model performed excpectionally well by acheibing a train accuracy of validation accuracy of 96.7 and test accuracy of 94.14

   
