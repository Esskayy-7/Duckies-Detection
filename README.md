# Duckies-Detection
This project demonstrates a YOLOv8 model detecting duckies in a Duckietown simulation video. The model is trained on a custom dataset and produces bounding boxes for detected duckies.

# Dataset
The model was trained using a custom dataset of 200(140 for training, 30 for validation and 30 for testing) with the YOLOv8 nano model, which I collected by myself and took factors like orientation, lighting and occlussion into consideration, The only preprocessing appplied was to standardize the sized of the images to 640x640.

# Peformance:
The model was trained for 100 epochs. Despite a limited training set (140 images), it achieved high localization and classification accuracy.Metric
Best ValueDescriptionmAP500.862Mean Average Precision. Indicates high reliability in detection.Precision0.873Accuracy of detections. Low false-positive rate.Recall0.807Detection coverage. Successfully identifies 80%+ of objects in frame.mAP50-950.321Precision at strict thresholds. Indicates decent bounding box alignment.
