**Project Goal**
I tried to build a video processor that classifies videos into different action categories using deep learning. The goal was to create a working pipeline for video classification
, from reading and processing video files to training and evaluating a model.

**Approach**
Processed each video file in a directory containing multiple categories of videos.
Padded each video to make sure all videos have similar frame counts.
Took the first 12 frames from each video since that is what my system could handle.
Standardized and normalized each frame.
Built a Conv3D-based neural network to train on the data.
Trained the model for 1 epoch due to system limitations.
Evaluated the model and attempted to predict the class of a new video.

**Dataset**
Used the UCF11 dataset which was available for free online.
Categories include basketball, biking, diving, golf swing, horse riding, soccer juggling, swing, tennis swing, trampoline jumping, volleyball spiking, and walking.
System Limitations
Due to system limitations i couldn't analyze each frame in each video using the network. I also had to reduce the number of frames to 12 and only train the network for 1 epoch.

**Results**
The network was able to train for 1 epoch and produce a prediction for a new video.
Because of the limited training, the results are not optimal but show that the end-to-end pipeline works.

**Future Work**
In future video classifiers when i have access to more advanced systems i'll add a more complete program. 
I will also try using more sophisticated pre-trained models and PCA to make the processor work better.
