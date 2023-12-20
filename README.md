# NYCUFall Dataset

The **NYCUFall** is a dataset of multi-view fall videos collected by 6 time-of-flight (ToF) depth cameras (Model 5Z01A, 5Voxel Co., Ltd.) in an indoor home environment. Please follow the [Open Database License](http://opendatacommons.org/licenses/odbl/1.0/) if you wish to use this dataset.



## Overview

This dataset contains depth frames captured from different camera perspectives in an indoor environment. The data is organized based on the camera perspective, datetime, and camera index.


## Inside This Dataset

* Image size: (H, W)=(172,224)
* Data type: `uint8`

### Sample Videos

<!-- - For **one sample** of **NYCUFall**, please check [here](./assets/NYCUFall_1sample.zip). -->


| Camera ID |   Video   | Camera ID |   Video   |
|:---------:|:---------:|:---------:|:---------:|
|ToF_1|<img src="assets/Figures/ToF1_sample01.gif" width="224" height="172"/>|ToF_2|<img src="assets/Figures/ToF2_sample01.gif" width="224" height="172"/>|
|ToF_3|<img src="assets/Figures/ToF3_sample01.gif" width="224" height="172"/>|ToF_4|<img src="assets/Figures/ToF4_sample01.gif" width="224" height="172"/>|
|ToF_5|<img src="assets/Figures/ToF5_sample01.gif" width="224" height="172"/>|ToF_6|<img src="assets/Figures/ToF6_sample01.gif" width="224" height="172"/>|


## Directory Hierarchy

The dataset follows the following directory structure:

- `Camera perspective`: `Ground` and `Top`
    - `Datetime`
        - `Camera index`


```
NYCUFall/
    ├── Ground/
    │   ├── 20211224_170408/
    │   │   ├── ToF_2/
    │   │   │   ├── 00000.png
    │   │   │   ├── 00001.png
    │   │   │   ├── 00002.png
    │   │   │   ├── 00003.png
    │   │   │   ├── 00004.png
    │   │   │   ├── 00005.png
    │   │   │   ├── ...
    │   │   ├── ...
    │   ├── ...
    │
    │
    ├── Top/
    │   ├── 20211224_170408/
    │   │   ├── 00000.png
    │   │   ├── 00001.png
    │   │   ├── 00002.png
    │   │   ├── 00003.png
    │   │   ├── 00004.png
    │   │   ├── 00005.png
    │   │   ├── ...
    │   ├── ...
```



## Labels or Categories

The labels for fall events are listed in individual csv file in both top view and side view.

- Top view: `label_Top_20231219.csv`

- Side view: `label_Ground_20231219.csv`


The dataset includes the following labels/categories in csv file:

- `Dir`: Datetime (`%Y%d%m_%H%M%S`)

- `subDir`: Camera index from `ToF_1` to `ToF_5`

- `FALLIndex`: The key frame of fall events (the frame that the person touches the ground)

- `Nobody`: A binary value. The value is 1 if there is no person in the video, and vice versa.



## File Formats

The file formats used in this dataset are:

- Video frame format: PNG files



## License

This **NYCUFall** dataset is made available under the [Open Database License](http://opendatacommons.org/licenses/odbl/1.0/) by National Yang Ming Chiao Tung University (NYCU). You can use, copy, transform and build upon the material for non-commercial purposes as long as you give appropriate credit by citing our paper (to be published in near future), and indicate if changes were made.

### Commercial Use

Commercial use of this dataset or any part thereof is strictly prohibited without prior written consent.

## Citation

The manuscript of this work is preparing.

Please cite the dataset using the appropriate reference when using it in your work. You may find the citation information in the dataset documentation.


## Link for Full Dataset

To be updated.

