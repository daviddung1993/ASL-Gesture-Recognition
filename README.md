# ASL-Gesture-Recognition

This repository shows the project that I have done in the Intelligent Interactive Systems course at Uppsala University. 
The project is about implementing a Convolutional Neural Network, that identifies gestures according to American Sign Language(ASL) standards.

The following gestures were implemented:

![ASL_letters](https://user-images.githubusercontent.com/38215056/160007116-e64a853d-f448-465c-ba07-6b19a67862b3.png)

Each student had to upload a video with hand gestures for each ASL letter, which was then aggregated to one Dataset. The Dataset is property of Ginevra Castellano, therefore it is not included in the repo. My videos are available as an example.

# Live demo

You can try out the model by running the demo notebook.
This would be an example output result:


https://user-images.githubusercontent.com/38215056/160009934-ba08d09e-bab0-4de6-8908-d15fd688d4c3.mov



# Process

- All of the videos were first split into frames
- Mediapipe was then used to detect the hand coordinates and crop the images
- Due to computational limitations, the images were then compressed to 32x32
- Videos 1-24 were the training set and video 25-29 were the test set
- Before feeding it to the CNN, data augmentation like flipping or 5% tilting was applied
- The overall accuracy of the model was ~83%




