# CustomHandGestureDetection

This project helps collect hand gesture data using MediaPipe, then train models using either Scikit-learn or MediaPipe Model maker

In order to collect custom Hand Gesture data, you have to run "Mediapipe-hand-gestures.ipynb". It will start using the webcam, and showing you the land marks of your hand. Create the gesture you want and press a key from 0-9 to label that gesture and save it. Click q to quit. This will output a folder named "data" containing the data in "gesture_data.csv". This file will organize the data with "x0, y0, z0, x1, y1, z1, ..., x20, y20, z20, label" as the header. There is more information about this code in the file: "Mediapipe Hand Data Collector Explained.pdf"

Now there are 2 ways to train the model: one method is to use Scikit-Learn (using "sklearnHandGestureModelMaker.ipynb"), which is a basic classifier, and will return a .pkl file; the other method is to use MediaPipe Model Maker (using "MpModelMakerHandGeasture.ipynb"), which will return two files: one for using on mobile (.tflite), and the other for real-time gesture detection using MediaPipe Tasks (.task).


