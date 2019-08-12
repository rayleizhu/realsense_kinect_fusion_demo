# realsense_kinect_fusion_demo
KinectFusion with realsense RGBD camera demo. It's based on [OpenCV4 KinFu API](https://docs.opencv.org/4.1.1/d8/d1f/classcv_1_1kinfu_1_1KinFu.html) and
[Intel RealSense Cross Platform API](https://github.com/IntelRealSense/librealsense/tree/v1.12.1),
tested with [Realsense ZR300](https://software.intel.com/en-us/realsense/zr300).

## Dependencies
[opencv-4.1.1](https://github.com/opencv/opencv)  
[librealsense-1.12.1](https://github.com/IntelRealSense/librealsense/tree/v1.12.1) [NOT librealsense2, their API are not compatiable]

## How to use
```
git clone https://github.com/rayleizhu/realsense_kinect_fusion_demo.git
cd realsensen_kinect_fusion_demo && mkdir build && cd build
cmake .. [-DCMAKE_PREFIX_PATH=/the/env/opencv4/installed/in/]
make
```
