# Sitting-Posture-Recognition
**A software that detects the sitting posture of a person in lateral view**

## Files
`model.py` - contains architecture of the model.

`config_reader.py` - contains the parameters that are essential for the model to predict the key points. 

`posture_image.py` - a static module that gives the output of an image.

`posture_realtime.py` - a dynamic module that gives the ooutput in realtime by analying the lateral view of the person through webcam.

## Usage 

1. Please install all the requirements from requirements.txt.
2. [Here](https://www.dropbox.com/s/llpxd14is7gyj0z/model.h5) is the trained keras model to detect the keypoints. You can download the model and save it under \model\keras folder.
3. Run `python3 posture_image.py` for testing this software with an image as input. If you wish to test it with your own image, put that image in `sample_images` folder and change accordingly on `line 243`. 
3. Run `python3 posture_realtime.py` for testing it in real time. Please sit sufficiently far away from the system showing your lateral view. Please note that this will require a system with atleast 8GB RAM. On a 4 GB RAM, the output is not at all smooth and the output lags very much from the input frame.
