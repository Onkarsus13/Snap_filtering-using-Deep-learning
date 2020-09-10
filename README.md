

A selfie filter implemented using Deep Learning and OpenCV

**Dataset:** https://www.kaggle.com/c/facial-keypoints-detection/data



Data from the dataset was augmented by flipping the images and their keypoints. I then used a CNN as the feature extractor, flattened the outputs and passed them into a fully connected ANN to perform facial keypoint regression. Metric used was 'Mean Absolute Loss', the model's best was ~0.0113 after being trained for 300 epochs using adam optimizer.

Once the model was complete, I used OpenCV to get live data from the webcam for real-time predictions. The input was preprocessed and input into the model and the outputs plotted. Then I used the positions of specific keypoints for the position and scale of 'filters'




