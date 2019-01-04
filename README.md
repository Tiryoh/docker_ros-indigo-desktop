# docker_ros-indigo-desktop

![](https://img.shields.io/docker/automated/tiryoh/ros-indigo-desktop.svg)
![](https://img.shields.io/docker/build/tiryoh/ros-indigo-desktop.svg)
![](https://img.shields.io/docker/pulls/tiryoh/ros-indigo-desktop.svg)

## Docker Hub

https://hub.docker.com/r/tiryoh/ros-indigo-desktop/

## Usage

* move into your ROS package, and just run:

  ```
  $ docker run --rm -it -v $(pwd):/ws tiryoh/ros-indigo-desktop catkin_make
  ```

  * `/ws` directory is simbolic linked to `/home/ubuntu/catkin_ws/src/ws`

* building ROS package `<package_name>` located in `~/workspace/ros/`:

  ```
  $ docker run --rm -it -v ~/workspace/ros/<package_name>:/home/ubuntu/catkin_ws/src/<package_name> tiryoh/ros-indigo-desktop catkin_make
  ```

* The default user of this container is `ubuntu` (not `root`), and the password is also set as `ubuntu`.

## License

The MIT License

2016-2018 (C) Tiryoh
