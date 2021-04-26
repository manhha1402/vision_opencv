vision_opencv
=============

.. image:: https://travis-ci.org/ros-perception/vision_opencv.svg?branch=indigo
    :target: https://travis-ci.org/ros-perception/vision_opencv

Packages for interfacing ROS with OpenCV, a library of programming functions for real time computer vision.

### Overlay

Build `vision_opencv` package with OpenCV built from source and Python3

`
catkin clean

catkin config -DPYTHON_EXECUTABLE=/usr/bin/python3 -DPYTHON_INCLUDE_DIR=/usr/include/python3.6m -DPYTHON_LIBRARY=/usr/lib/x86_64-linux-gnu/libpython3.6m.so --install

catkin build -DCMAKE_BUILD_TYPE=Release
`

Check installation:

`
python3

from cv_bridge.boost.cv_bridge_boost import getCvType
`

