# Object Detection with YOLO
## Instructions
Generate yolo.h5 with `python yad2k.py model_data/yolo.cfg model_data/yolo.weights model_data/yolo.h5`
Install `requirements.txt`
Run `yolo.ipynb`

## Overview
This project involved implementing object detection using the YOLO (You Only Look Once) model, a powerful approach described in the papers by Redmon et al., 2016, and Redmon and Farhadi, 2016. The main objective was to detect objects in a car detection dataset by handling bounding boxes, applying non-max suppression for accuracy improvement, and utilizing intersection over union. These techniques are pivotal in image annotation, a common task in deep learning. This project follows the steps outlined in the following DeepLearning.Ai course: [Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning).

## Implementation Details

- **YOLO Model:** The core of this project was to understand and implement the YOLO algorithm, known for its efficiency and effectiveness in detecting objects by looking at the image only once.
- **Bounding Boxes:** Learned how to handle bounding boxes, which are essential for locating objects within images.
- **Non-max Suppression (NMS):** Implemented NMS to reduce the number of overlapping boxes, thereby improving the detection accuracy.
- **Intersection Over Union (IoU):** Utilized IoU to measure the overlap between predicted boxes and ground truth, which helps in evaluating the model's performance.

## Technical Achievements

- **Detection in Car Dataset:** Successfully applied the YOLO model to detect vehicles in a dataset collected from a car-mounted camera, showcasing the model's potential in real-world applications like self-driving cars.
- **Model Adjustments:** Adapted the YOLO model, originally trained on a different size, to work with images of size 608x608 by understanding and manipulating the model's inputs and outputs.
- **Algorithm Understanding:** Gained a deep understanding of the YOLO algorithm's inner workings, including how it processes images through a deep CNN to predict bounding boxes and class probabilities.

## Challenges and Learnings

- **Model Implementation:** The source code and instructions for this project were outdated to modern versions of TensorFlow and Keras. Substantial adjustments were made to the base libraries to ensure compatibility with the current versions.
- **Algorithm Complexity:** One of the main challenges was to grasp the complex nature of the YOLO algorithm, especially its unique way of predicting multiple bounding boxes and class probabilities simultaneously.
- **Optimization Techniques:** Learned about advanced optimization techniques like NMS and IoU, which are crucial for enhancing the model's detection accuracy by filtering out redundant boxes.
- **Tensor Manipulation:** Gained substantial experience in manipulating tensors to reshape and filter the model's outputs, a skill that is widely applicable in deep learning tasks.

## Conclusion

This project was a comprehensive introduction to object detection using YOLO, from understanding the theoretical aspects to implementing the model on a specific dataset. The experience has solidified my understanding of important concepts like bounding boxes, NMS, and IoU, while also highlighting the practical challenges and considerations in applying such a model to real-world tasks.

### References

- Redmon, J., Divvala, S., Girshick, R., & Farhadi, A. (2016). You Only Look Once: Unified, Real-Time Object Detection.
- Redmon, J., & Farhadi, A. (2016). YOLO9000: Better, Faster, Stronger.
- Allan Zelener - YAD2K: Yet Another Darknet 2 Keras
- The official YOLO website (https://pjreddie.com/darknet/yolo/) for YOLOv2 weights and configuration files.
