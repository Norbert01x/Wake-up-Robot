# Wake-up-Robot
This Robot won't let you sleep

Almost all of us experienced falling asleep while doing something like reading a book.
so I built a robot that based on face and eyes detection can know you're falling asleep and it can wake you up.

In this project I used eSpeak To give the robot ability to speak and OpenCV for image processing.
eSpeak is a compact open source software speech synthesizer for English and other languages.
OpenCV (Open Source Computer Vision Library) is an open source computer vision and machine learning software library.
OpenCV was built to provide a common infrastructure for computer vision applications and to accelerate the use of machine perception in the commercial products.

The way image recognition works is we first need to "train" a classifier.

To do this, we generally need to compile a massive set of images of what we're looking to detect (In this case face and eyes).  OpenCV already contains many pre-trained classifiers for face, eyes, smile etc. Those XML files are stored in opencv/data/haarcascades/ folder. in this project we need haarcascade_frontalface_alt.xml and haarcascade_eye_tree_eyeglasses.xml.
After training it checks if there is face in the frame or not. then checks if there is opened-eyes or not. 
For best results you may need to change detectmultiscale parameters.

YouTube Video: https://youtu.be/KtnHZ2SUYKc
