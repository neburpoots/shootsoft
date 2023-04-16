# Shootsoft model and dataset

This repository contains the Shootsoft model and dataset. The model is a deep neural network that predicts the amount of points scored on a target. The dataset contains around 2100 annotated images with the correct scores. The model can be found in the `runs/detect/train/weights` folder. The correct model to use is the best.pt. The model is trained by making use of Yolov8. Yolov8 is a popular object detection alghorithm. It uses and end-to-end neural network that makes predictions of bounding boxed and class probabilities at the same time. The Yolov8 architecture differs from standard RCNN by making use of a series of convolutional layers followed by one fully connected layer. The model is trained on 100 epochs. The reason for training the model for 100 epochs was done because of the val/cls_loss. Below is a table with the results of the model. A more extensive overview over the metrics of the models can be found in the `runs/detect/train` this also contains a confusion matrix for every individual class.

## Metrics

Statistic                   | Value
----------------------------| -------------
F1-Confidence               | 0.91
Recall Confidence           | 0.98
metrics/precision           | 0.91321
metrics/mAP50(B)            | 0.94839
metrics/recall(B)           | 0.90001

Statistics (last epoch) | Validation | Training
------------------------| ---------- | ---------
cls_loss                | 0.41581    | 0.26985
box_loss                | 0.88657    | 0.51291
dfl_loss                | 0.91771    | 0.82919
dfl_loss                | 0.91771    | 0.82919


## Roboflow

The model dataset can be found on https://app.roboflow.com/project-bat/project-oqaxk/overview

## Technicalities

The model is trained with python 3.10.7 and requires ultralytics version 8.0.58 to function properly.

## Division of tasks

The contribution of each team member on all of the content in this repository can be found in the : `log`

## Technical Functional and Graphical Design for the Proof of concept

To further explain the technical functional and graphical design of the proof of concept, we have created a document called TFGD folder. This document contains a description of the proof of concept, the technical functional and graphical design of the proof of concept and a description of the user interface.


## License

All contents of this repository is licensed under a GPL-3.0 license. See the LICENSE file for more information.