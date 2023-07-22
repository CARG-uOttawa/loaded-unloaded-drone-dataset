# Loaded-unloaded-drone-dataset

Simulated Dataset Using AirSim for the Loaded vs. Unloaded UAV Classification Problem

# Dataset
The dataset is accessible through this link (the link will be provided just after the presentation of the paper in SAS 2023 in July 2023).

# Annotation files
Each video is accompanied by an annotation file that contains the following information on each line:

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


