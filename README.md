# Duckies-Detection
This project demonstrates a YOLOv8 model detecting duckies in a Duckietown simulation video. The model is trained on a custom dataset and produces bounding boxes for detected duckies.

# Dataset
The model was trained using a custom dataset of 200(140 for training, 30 for validation and 30 for testing) with the YOLOv8 nano model, which I collected by myself and took factors like orientation, lighting and occlussion into consideration, The only preprocessing appplied was to standardize the sized of the images to 640x640.

# Peformance:
The model was trained for 100 epochs. Despite a limited training set (140 images), it achieved high localization and classification accuracy.

## Model Evaluation Metrics

| Metric      | Best Value | Description                                           |
|------------|------------|-------------------------------------------------------|
| mAP50      | 0.862      | Mean Average Precision. Indicates high reliability in detection. |
| Precision  | 0.873      | Accuracy of detections. Low false-positive rate.    |
| Recall     | 0.807      | Detection coverage. Successfully identifies 80%+ of objects in frame. |
| mAP50-95   | 0.321      | Precision at strict thresholds. Indicates decent bounding box alignment. |

# Observations / Current Limitations
The current model works best when the duckies appears to be in motion but not when stationary and is better at detecting obects close by and not far away. The biggest limitation is the small dataset and I will be using more for training next time allong with some augmentation for better results

# link to dataset and output
https://drive.google.com/drive/u/0/folders/10ywTOSWbLAqYamevZS1HSksRhYawc8wB

