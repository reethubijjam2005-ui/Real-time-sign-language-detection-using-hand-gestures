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
STEP 2: Model Training
python train_model.py What happens:

Loads all collected data (800 samples)
Splits into training (80%) and testing (20%)
Trains SVM classifier on training data
Tests accuracy on testing data
Saves trained model Why needed: • SVM learns patterns from hand landmarks • Creates decision boundaries between different signs • Validates model performance before deployment Output: • Creates sign_language_model.pkl file • Shows accuracy score (aim for >90%) • Shows classification report for each sign
STEP 3: Real-time Detection python detect_signs.py What happens:

Loads trained model
Opens webcam
Detects hand in real-time
Predicts sign language gesture
Shows prediction with confidence Why needed: • Deploys the trained model • Provides real-time user interaction • Smooths predictions for stable display Output: Live video with sign predictions Press 'q' to quit

