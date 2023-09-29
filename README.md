# Loaded-unloaded-drone-dataset

Detecting payloads on Uncrewed (or Unmanned) Aerial Vehicles (UAVs) is crucial for safety and security reasons. Deep learning methods can utilize changes in UAV appearance caused by payloads for detection, but collecting sufficient training data through real tests is costly and time-consuming. Therefore, simulation can be a more practical option. This page presents the first synthetic air-to-air vision dataset for classifying loaded vs. unloaded UAVs. The dataset includes five types of aerial vehicles (_DJI Phantom, DJI Mavic, DJI FPV, DJI Inspiron, and a generic quadrotor model_) with attached and hanging payloads of different colors. It also incorporates three environments (_Blocks, Landscape Mountains, City Park-Lite_) and environmental conditions (_sunny, rainy, and snowy_) to diversify the background in recorded videos. Annotated frames and XYZ coordinates of the camera and drone are provided. 

# Dataset
The dataset is accessible through this link (the link will be provided just after the presentation of the paper).

# Annotation files
The videos are recorded at a resolution of 1080x1920 pixels, and a frame rate of 10 fps. The pixel indexing starts from (1, 1) at the top-left corner and goes up to (1080, 1920) at the bottom-right corner. Each video is accompanied by an annotation file that contains the following information on each line:

[`Frame number` `Detection flag` `Xtl` `Ytl` `Xbr` `Ybr` `Xcamera` `Ycamera` `Zcamera` `Xdrone` `Ydrone` `Zdrone`]

where:
* `Frame number`: integer value that starts from 1 and shows the frame index
* `Detection flag`: the flag indicates whether the drone exists in that frame or not (0 or 1, where 1 means that the drone exists)
* `Xtl` and `Ytl`: the position of the top-left corner of the drone's bounding box in pixels (integer value, starts from 1)
* `Xbr` and `Ybr`: the position of the bottom-right corner of the drone's bounding box in pixels (integer value, starts from 1)
* `Xcamera`,`Ycamera`, and `Zcamera`: the coordinates of the camera's location in the AirSim's internal Cartesian coordinate frame (meters)
* `Xdrone`, `Ydrone`, and `Zdrone`: the coordinates of the camera's location in the AirSim's internal Cartesian coordinate frame (meters)



# Citation
If you use this dataset for your work, please cite the following paper:
```
@InProceedings{azad2023simulated,
    author    = {Azad, Hamid and Mehta, Varun and Bolic, Miodrag and Mantegh, Iraj},
    title     = {Simulated Dataset for the Loaded vs. Unloaded UAV Classification Problem Using Deep Learning},
    booktitle = {2023 IEEE Sensors Applications Symposium (SAS)},
    month     = {July},
    year      = {2023},
    pages     = {1-6}
}
``` 


