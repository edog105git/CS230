# Detecting Infarct Cores in Acute Ischemic Stroke from CT with Deep Learning
We aim to construct a deep learning model that reads non-contrast material-enhanced CT (NCCT) images of the brain and performs segmentation of acute ischemic stroke tissue.
## Pre-processing
The data used for this project is taken from the Ischemic Stroke Lesion Segmentation [(ISLES) challenge dataset](https://www.smir.ch/ISLES/Start2018). Baseline CT perfusion (CTP) slices for different patients in the original dataset were processed using [*Read_ISLES_Data.ipynb*](Read_ISLES_Data.ipynb) to form 436 input NCCT images of size 256 x 256, with corresponding 436 label segmentation images of size 256 x 256. The dataset can be augmented by applying horizontal mirroring using [*mirror.ipynb*](mirror.ipynb).
## Baseline model
The baseline deep learning model employed is a U-Net architecture. This is implemented and tested to obtain results in [*Test_Unet_baseline.ipynb*](Test_Unet_baseline.ipynb).
## Symmetry-encoded model
We employ a symmetry-encoded U-Net as a second approach to the proposed deep learning task. This is implemented and tested to obtain results in [*Test_Unet_Symmetry_arm.ipynb*](Test_Unet_Symmetry_arm.ipynb).
## Modified symmetry-encoded model
We modify the symmetry-encoded model as a third approach. This is implemented and tested to obtain results in [*Test_Unet_Symmetry_arm_flip_connect.ipynb*](Test_Unet_Symmetry_arm_flip_connect.ipynb). 
