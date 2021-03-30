# eye_blinking_detection_and_counting_system
This program is developed in python programming language. It was intended to count human eye blinks. This application is very useful for sleeping detection and other medical related problems.

# Download Shape Predictor

shape predictor() is a tool that takes in an image region containing some object and outputs a set of point locations that define the pose of the object.
shape_predictor_68_face_landmarks.dat is a useful tool, it returns facial features locations as coordinates. 
[Download Link:](https://osdn.net/projects/sfnet_dclib/downloads/dlib/v18.10/shape_predictor_68_face_landmarks.dat.bz2/)


# Dependencies
- Python 3.6
- OpenCV
- Scipy
- Dlib
- Scipy


# Command Line Arguments

```

ap = argparse.ArgumentParser()
ap.add_argument("-p", "--shape-predictor", required=True,
	help="path to facial landmark predictor")
ap.add_argument("-v", "--video", type=str, default="",
	help="path to input video file")
args = vars(ap.parse_args())

```

# How to run this program

```

python detect_blinks.py -p shape_predictor_68_face_landmarks.dat -v test.m4v 

```