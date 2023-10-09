# BleedDetect-CapsuleEndoVision  

This README provides an overview of the work done in the Bleeding Cell Detection project. The project involves data augmentation, training a YOLOv8 model, and evaluating its performance on bleeding cell detection.

## Data Augmentation
The first step of the project involved augmenting the dataset of bleeding cell images and non-bleeding cell images. This augmentation was performed by rotating the images at various angles, including 90°, 180°, 270°, 22°, 44°, 66°, 88°, 110°, 132°, 154°, 176°, 198°, 220°, 242°, 264°, 286°, 308°, 330°, and 352°. Corresponding labels were created for each augmented image.

## Data Splitting
The augmented data, along with the original images and labels, was split into testing, training, and validation sets. The data splitting was done with a 20% allocation to the testing folder, 10% to the validation folder, and 70% to the training folder.

## Model Training
The YOLOv8 model was chosen for this project. The training data was used to train the model for 200 epochs. We saved the weights after each epoch to track the model's progress. The best-performing weight was selected for further evaluation and saved in the weights folder.
Testing and Evaluation
Using the best weight obtained during training, we tested the model's performance on the test data. We achieved predictions for bleeding cell images with confidence metrics.

## Classification Metrics
•	Accuracy
•	Recall
•	F1-Score

## Detection Metrics
•	Average Precision
•	Mean-Average Precision (mAP)
•	Intersection over Union (IoU)
The evaluation metrics, including the IoU values, for images during training are available in the "evaluation_metrics" folder. Specifically, the IoU values during training are stored in "iou_during_training.xlsx". The IoU values during testing with the given dataset 1 are available in the same folder as "Test_data_img_IOU.xlsx".

## Visualizations
In the "pictures" folder, you will find various visualizations:
Validation Dataset
•	Screenshots/pictures of the 10 best images from the validation dataset, showing classification and detection with bounding boxes and confidence levels.
•	Achieved interpretability plots for 10 selected images from the validation dataset.

## Testing Datasets 1 and 2
•	Screenshots/pictures of the 5 best images from testing dataset 1, showing classification and detection with bounding boxes and confidence levels.
•	Screenshots/pictures of the 5 best images from testing dataset 2, showing classification and detection with bounding boxes and confidence levels.
•	Achieved interpretability plots for 5 selected images from testing datasets 1 and 2.




This README summarizes the key steps and outcomes of the Bleeding Cell Detection project. For detailed results and additional information, please refer to the respective folders and files in the project directory.

