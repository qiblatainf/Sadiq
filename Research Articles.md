# Sadiq

# Strategy 1

Step Wise Approach:

Link: (https://www.researchgate.net/publication/358201557_A_Deep_Learning-Based_Approach_for_Inappropriate_Content_Detection_and_Classification_of_YouTube_Videos)

## 1. Video Pre-Processing

1. A video (Vi) is ﬁrst represented as N small segments of videos referred to as video clips (ci1,ci2, . . . ., ciN) with one-second length each (the length can vary)
2. We split the frames and label them
3. Duplicate frames and irrelevant frames are eliminated or the time frame is changed
4. The selected frames of each video clip are re-scaled to a ﬁxed resolution of 224 ×224 pixels that correspond to the input size of the pre-trained convolutional neural network model

## 2. Deep Feature Extraction

1. EfficientNetB7 - to extract video descriptors (feature extraction) which is a pre-trained CNN architecture
2. The feature vectors are reshaped

## 3. Video Classification

1. The descriptors are fed to BiLSTM (bi-directional long short-term memory) for better video representation and multi-class video classification.
2. Softmax Layer is used as a classifier

Accuracy: 95.66

# Strategy 2

Link: https://www.researchgate.net/publication/336430665_A_baseline_for_NSFW_video_detection_in_e-learning_environments

Theirr CNN-based SFW/NSFW classier is composed by two modules:
1. Feature Extractor
2. Classifier
Once we have extracted the features from the video, we then use a shallow model to performthe video classication. 

# Strategy 3
Model Name: MobileNetV3
Article: https://arxiv.org/pdf/2107.11845.pdf

General: https://github.com/abbasidaniyal/Wikimedia-NSFW-Classifier-Reports/blob/dc7a4192eda23b067c85a131f5502514b9bf4222/reports/Abhipsha%20Das%20-%20Microtasks/T264056%20-%20NSFW%20Classifiers%20Comparison.ipynb
