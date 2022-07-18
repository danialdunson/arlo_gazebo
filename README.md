# arlo_gazebo
This package simulates the Parallax Arlo Robot in Gazebo. 

Please use `Gazebo Version> 9.19.x+`

Download the following packages and place them in your workspace.

|Required Packages    |  Link                                                                                   |
|--------------       | ----------                                                                              |
| aws-house           | [repository](https://github.com/aws-robotics/aws-robomaker-small-house-world)           |
| realsense plugin    | [repository](https://github.com/pal-robotics/realsense_gazebo_plugin)                   |

# Running the Simulation

* Start the simulation with the following command:
```bash
roslaunch arlo_gazebo arlo_sim.launch
```
Press tab to see the available options.

![This is an image](/resources/images/Press_tab_to_view_launch_args.png)

There are 19 args are available in the launch file to modify as in command line.

Please visit the [launch folder](/launch/README.md) for more information.

|Argument               | description                           | default                   |
|-----------------------|:-------------------------------------:|--------------------------:|
|x_pos, y_pos, z_pos    | Set robot spawn location              | (-1.33, 0.55, 0.02)       |
|use_rtabmapviz         | Enable rtabmap GUI visualization      | false                     |
|ns                     | Namespace for the entire robot        | wx250s                    |
|arlo_rviz              | Visualize the Arlo Robot in RViz      | true                      |
|isolate                | Minimal startup                       | false                     |
|teleop                 | Launch teleop_keyboard node           | false                     |




## View of the Arlo Robot running in RViz.
![This is an image](/resources/images/rviz_gazebo.png)

## Example of populated rtabmap/MapData in RViz.
![This is an image](/resources/images/MapData_after_mapping.png)

## View of Rtabmap in GUI.
Set the `use_rtabmapviz` argument to `true` in the launch file.

In Rtabmap-GUI, enable mapping to populate the rtabmap/MapData as shown in the image below.

![This is an image](/resources/images/rtabmapviz_enable_mapping.jpg)


