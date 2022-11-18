# multi_nav

Navigation for multi robots using Nav2 ros package.


## dependencies

```
sudo apt-get install ros-foxy-nav2-map-server
```
## Usage

we used the launch file from this [site](https://answers.ros.org/question/398095/ros2-nav2-map_server-problems-loading-map-with-nav2_map_server/)

```
ros2 launch multi_nav2 make_map.launch.py
ros2 launch nav2_bringup bringup_launch.py use_sim_time:=False autostart:=False map:=path_to_pkg/multi_nav2/param/map.yaml
```