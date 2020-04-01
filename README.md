>If you are unable to view the IPYNB notebook in GitHub, Please copy the GitHub notebook URL and paste it in [nbviewer](https://nbviewer.jupyter.org/).

# Semantic Segmentation Challenge on Indian Driving Dataset 

#  Business Problem
###  Description
While several datasets for autonomous navigation have become available in recent years, they have tended to focus on structured driving environments. This usually corresponds to well-delineated infrastructure such as lanes, a small number of well-defined categories for traffic participants, low variation in object or background appearance and strong adherence to traffic rules. We propose a novel dataset for road scene understanding in unstructured environments where the above assumptions are largely not satisfied.

The dataset consists of images obtained from a front facing camera attached to a car. The car was driven around Hyderabad, Bangalore cities and their outskirts. 

### Challenge
The segmentation challenge involves pixel level predictions for all the 7 classes at level 1 of the label hierarchy on IDD Lite (IDD-Lite, a dataset that is small and compact to fit on any personal computer and so will not huge-compute infrastructure) [Refer here](https://github.com/AutoNUE/public-code/blob/312a6ba2219a39fe8b105e44ad0612079249bad8/helpers/anue_labels.py#L40)

These 7 classes include Drivable, Non-Drivable, Living things, Vehicles, Road side objects, Farobjects , Sky
## Type of Problem

- Semantic Segmentation

## Performance Metric

 mean Intersection over Union(mIoU) [Refer Here](https://towardsdatascience.com/metrics-to-evaluate-your-semantic-segmentation-model-6bcb99639aa2)
 
 ## Dataset Overview

- Shape of the input image and segmentation masks given: [227,320,3]

- Shape of the output segmentation mask expected: [128,256]

We have 1403 train images , 204 validation images and 404 test images
## Methods
- UNet (Obtained best results)
- DeepLab v3+

## Results

Observed mIoU of 0.72 on Train data and 0.61 on Validation data respectively. 

Generated Semantic Segmentaion maps for test data

