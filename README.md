# Object Detection with OpenCV (cv2)
This project demonstrates object detection using OpenCV (cv2) with a pre-trained SSD MobileNet V3 model. The model is capable of detecting various objects from the COCO dataset, such as cars, people, and animals.

Components
Configuration Files: Uses ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt for model configuration and frozen_inference_graph.pb for the trained model weights.

Model Initialization: Initializes the object detection model (cv2.dnn_DetectionModel) with the configuration and frozen model files.

Class Labels: Loads class labels from labels.txt, which defines the categories of objects the model can detect.

Image Processing: Reads an image (img) using OpenCV (cv2.imread) and displays it using Matplotlib (matplotlib.pyplot.imshow).

Object Detection: Utilizes the initialized model to detect objects in the image (model.detect). It returns class indices, confidence scores, and bounding box coordinates for detected objects.

Visualization: Draws bounding boxes and labels around detected objects on the image using OpenCV (cv2.rectangle, cv2.putText) and displays the annotated image using Matplotlib.

Usage
Setup: Ensure Python environment with OpenCV (cv2) and Matplotlib installed.

Run: Execute the script to load the model, detect objects in the specified image (img), and visualize the results.
