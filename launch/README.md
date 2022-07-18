# Arlo_sim.launch
|Argument               | description                           | default                   |
|-----------------------|:-------------------------------------:|--------------------------:|
| | __Most used arguments__ | |
|x_pos, y_pos, z_pos    | Set robot spawn location              | (-1.33, 0.55, 0.02)       |
|use_rtabmapviz         | Enable rtabmap GUI visualization      | false                     |
|ns                     | Namespace for the entire robot        | wx250s                    |
|arlo_rviz              | Visualize the Arlo Robot in RViz      | true                      |
| |                  __Gazebo args__                                                        |                  
|gui                    | Enable the Gazebo GUI                 | true                      |
|debug                  | Enable debug mode                     | true                      |
|paused                 | Start the simulation paused           | true                      |
|recording              | Enable recording of the simulation    | false                     |
|world name             | Name of the world file                | /worlds/small_house.world |
|extra_gazebo_args      | Additional Gazebo args                |   ' '                     |
| |                   __URDF args__                                                         |
|robot_name             | Model of the robot (sets frame ns)    | wx250s                    |
|model                  | Model of the camera                   | realsense                 |
|base_link_frame        | Base link frame for the arm           | arm_base_link             |
|arm                    | Enable the arm                        | false                     |
|update_rate            | Update rate for the camera            | 15                        |
|robot_name             | Name of the robot                     | wx250s                    |
|isolate                | Minimal startup                       | false                     |
|rviz_frame             | Fixed Frame in Rviz                   | wx250s/map                |

# TF Tree (without wx250s)
```bash
rosrun rqt_tf_tree rqt_tf_tree
```

![This is an image](/resources/images/tf_tree.png)