# Finetuning YOLOv8 for Product Object Detection

In this study, we fine-tuned YOLOv8 model for object detection using a custom training dataset, then used the fine-tuned model to make predictions on the test set and generate a submission file for Kaggle.

## Steps:

### 1. Data Preparation:

- We loaded the training dataset and encoded class names into numeric labels.  
- We converted the bounding box format from XYXY (corner points) to YOLO's normalized format (center, width, height).  
- We saved the images and labels in the required format for YOLO training.  

### 2. YOLOv8 Model Fine-Tuning:

- We loaded a pre-trained YOLOv8 model and fine-tuned it on our custom dataset for object detection.

### 3. Inference on Test Set:

After fine-tuning, we used the model to make predictions on the test set.  
The predictions included object class labels, confidence scores, and bounding boxes.

### 4. Submission File:

- We formatted the predictions into a CSV file with image_id and prediction_string columns.  
- The prediction_string contains detected classes, their confidence scores, and bounding boxes in the required format for submission.