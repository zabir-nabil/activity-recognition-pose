# activity-recognition-pose
Human Activity Recognition from Skeletal data (Pose)

### Dataset
https://gitlab.com/zabir-nabil/datasets/tree/master/dance%20activity%20recognition

* The original dataset is from https://www.cc.gatech.edu/cpl/projects/dance/

* The image frames have been processed with a multi-subject pose estimation model https://github.com/zabir-nabil/keras-human-pose

* 4 classes from the original dataset are used ('break', 'ballet', 'cha', 'flamenco')
* In the data folder, there are 4 sub-folders named ('break', 'ballet', 'cha', 'flamenco')
* In each folder, there are many .npy files
* Each numpy file represents a frame
* Each file has the name format X_Y_Z.npy
* Here, X is the id of a specific dance activity (video)
* Y denotes the id of the frame of activity X
* Z denotes the class of activity
* Each numpy (.npy) file contains an array with shape (body parts, subject, X coordinate, Y coordinate)
* Body parts mapping => [nose, neck, Rsho, Relb, Rwri, Lsho, Lelb, Lwri, Rhip, Rkne, Rank, Lhip, Lkne, Lank, Leye, Reye, Lear, Rear]
* If a joint is missing for a subject the coordinates are (-1,-1)
