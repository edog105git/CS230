# CS230
We aim to construct a deep learning model that reads non-contrast material-enhanced CT (NCCT) images of the brain and performs segmentation of acute ischemic stroke tissue.
## Pre-processing
The data used for this project is taken from the Ischemic Stroke Lesion Segmentation [(ISLES) challenge dataset](https://www.smir.ch/ISLES/Start2018). Baseline CT perfusion (CTP) slices for different patients in the original dataset were processed using [*Read_ISLES_Data.ipynb*](Read_ISLES_Data.ipynb) to form 436 input NCCT images of size 256 x 256, with corresponding 436 label segmentation images of size 256 x 256. The dataset can be augmented by applying horizontal mirroring using [*mirror.ipynb*](mirror.ipynb).
## Baseline model
The baseline deep learning model employed is a U-Net architecture. This is implemented and tested to obtain preliminary results in [*Test_SegNet.ipynb*](Test_SegNet.ipynb).
