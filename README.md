# docker_ros-indigo-desktop

![](https://img.shields.io/docker/automated/tiryoh/ros-indigo-desktop.svg)
![](https://img.shields.io/docker/build/tiryoh/ros-indigo-desktop.svg)
![](https://img.shields.io/docker/pulls/tiryoh/ros-indigo-desktop.svg)

## Docker Hub

https://hub.docker.com/r/tiryoh/ros-indigo-desktop/

## Usage

building ROS package `<package_name>` located in `~/repo/ros_ws/`:
```
$ docker run --rm -it -v ~/repo/ros_ws/<package_name>:/home/ubuntu/catkin_ws/src/<package_name> tiryoh/ros-indigo-desktop catkin_make
$ 
```

## License

The MIT License

2016-2018 (C) Tiryoh
