# Yolo Model Analysis

# Baseline Model

The baseline model YOLOv11 was trained on the VisDrone dataset. Here the results.

![](figures/baseline/compare.png)

This graph showcases key statistics from the validation and training set of data. Importantly we are using the mosaic augmentation. This parameter during the training stage will combine four images into one. This ensures that model learns on the image content itself, rather than arbitrary features. This augmentation is why validation loss is lower than the training, until mosaic is dropped in epoch 40.

We can see that this model showcased a normal training stage. The model made siginicant progress in epochs 1-30, and then started to plateu. Importantly, the model still imporved in higher epochs. This hints that the model may be slightly underfitted to the problem. Yet, this does not change that for this model archicture and dataset we have roughly around a 0.50 mAP celiing.
