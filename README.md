# Automated Pituitary Adenoma Segmentation for Radiosurgical treatment Planning
This is a code repository accompanying the article **Utility of Artificial Intelligence in Radiosurgery for Pituitary Adenomas: A Deep Learning-Based Automated Segmentation Model with Evaluation of its Clinical Utility**Černý M., May J., Hamáčková L., Novotný J., Baručić D., Kybic J., Májovský M., Hallak H., Balasubramaniam N., Liščák R. and Netuka D.

This program and/or it's parts are not intended for clinical use
If zou use this code, please cite our article

## Usage:

This repository contains two nnU-net models for pituitary adenoma segmentation
For general instructions on how to use nnU-net see [here](https://github.com/MIC-DKFZ/nnUNet)

005 - uses coronal contrast-enhanced T1-weighted and coronal T2-weighted MRI scans as input
006 - uses coronal contrast-enhanced T1-weighted only as input

Copy these models to the results folder of nnU-net on your computer

Run the inference by calling:

```
nnUNetv2_predict -i [INPUT_FOLDER] -o [OUTPUT_FOLDER] -d 5 -c 3d_fullres -f 1
```

Please note that only fold 1 is trained