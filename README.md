# docker_ros-indigo-desktop
ros-indigo-desktop Ubuntu14.04

# Sample

```
socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\"
```

```
docker run -it --rm -h docker --name ros --env DISPLAY=192.168.99.1:0 -v $HOME/repo/ROS/ws/catkin_ws/src:/home/ubuntu/catkin_ws/src tiryoh/ros-indigo-desktop
```

```
docker exec -it ros /bin/bash
```

