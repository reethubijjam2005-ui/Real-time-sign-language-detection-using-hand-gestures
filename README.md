# Real-time-sign-language-detection-using-hand-gestures
SIGN LANGUAGE DETECTION USING HAND GESTURE

INTRODUCTION: In the current world there are people who is disabled like hearing problem or cannot speak. So this is a mini project used to bridge the gap between them and the normal people, in machine learning domain using python as the programming language and SVM (support virtual machine) algorithm.

SOFTWARE REQUIRED: • Pycharm or Jupiter notebook. • Python version of 3.7 or 3.8. • opencv-python: Camera access and image processing • mediapipe: Hand detection and landmark extraction (21 points per hand) • numpy: Numerical operations on data arrays • scikit-learn: Machine learning (SVM algorithm)

HARDWARE REQUIRED: • Laptop or PC. • Webcam.

STEP 1: Data Collection python collect_data.py What happens:

Webcam opens showing your hand
For each of 8 words, perform the sign gesture
Press 's' to start collecting 100 samples
Move hand slightly while maintaining the sign
Repeat for all 8 words Why needed: • Collects 100 samples per sign (800 total) • Each sample = 63 features (21 landmarks × 3 coordinates) • More samples = better accuracy Output: Creates sign_data/ folder with 8 .pkl files.
