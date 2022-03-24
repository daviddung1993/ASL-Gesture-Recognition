# ASL-Gesture-Recognition

This repository shows the project that I have done in the Intelligent Interactive Systems course at the Uppsala University. 
The project is about implementing a Convolutional Neural Network, that identifies gestures according to American Sign Languague(ASL) standards.

The following gestures were implemented:

![ASL_letters](https://user-images.githubusercontent.com/38215056/160007116-e64a853d-f448-465c-ba07-6b19a67862b3.png)

Each student had to upload a video with hand gestures for each ASL letter, which was then aggregated to one Dataset. The Dataset is property of Ginevra Castellano, therefore it is not included in the repo. My videos are available as an example.

# Live demo

You can try out the model by running the demo notebook.
This would be an example output result:
https://user-images.githubusercontent.com/38215056/160008232-5681042a-f4ec-4fdd-bf75-1a3328c2f10a.mp4

# Process

- All of the videos were first split into frames
- Mediapipe was then use to detect the hand coordinates and crop the images
- Due to computational limitations, the images were then compressed to 32x32
- Video 1 to 24 were the training set and video 25-29 were the test set
- Before feeding it to the CNN, following data augmentation like flipping or a 5% tilt was applied
- The overall accuracy of the model were ~83%




