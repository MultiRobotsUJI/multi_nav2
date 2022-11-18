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
```

From this [site](https://navigation.ros.org/tutorials/docs/navigation2_on_real_turtlebot3.html) we do:

```
ros2 launch nav2_bringup bringup_launch.py use_sim_time:=False autostart:=False map:=path_to_pkg/multi_nav2/param/map.yaml
```

```
ros2 run rviz2 rviz2 -d $(ros2 pkg prefix nav2_bringup)/share/nav2_bringup/rviz/nav2_default_view.rviz
```