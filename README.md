# Process Setup Waypoints

The Waypoint Navigation Plugin is a tool for the Robot Operating System (ROS) that allows users to specify multiple waypoints in the ROS Visualization (Rviz) environment and then save to a file in `yaml` format for use with RNS (Robot Navigation System) or other navigation systems.

## Prerequisites
-   ROS installation (instructions can be found [here](http://wiki.ros.org/ROS/Installation))
-   Rviz installation (instructions can be found [here](http://wiki.ros.org/rviz))

## Launching the Waypoint Navigation Plugin
```bash
roslaunch waypoint_navigation_plugin rviz.launch
```
This will open Rviz with the Waypoint Navigation Plugin added as a tool.

To specify the name of the map to which you want to add or modify waypoints, you can provide the map_name argument in the roslaunch command as follows:
```bash
roslaunch waypoint_navigation_plugin rviz.launch map_name:=<name of map>
```
For example, to use the bookstore map, you would use:
```bash
roslaunch waypoint_navigation_plugin rviz.launch map_name:=bookstore
```
## Adding and Editing Waypoints
To add waypoints, click on the Waypoint Navigation Tool in the Rviz toolbar, and then click on the Rviz scene to place a waypoint. You can add multiple waypoints by repeating this process.

To update the location of a waypoint, you can either drag the interactive marker associated with the waypoint, or use the Rviz panel to specify the new position.

<div align="center">
     <img src="doc/wp_doc_002.png" alt="Rviz" width="650px">
</div>

## Save Waypoints

To save waypoints that have been added in Rviz, first click on the desired waypoint in the Rviz tool. Then save the waypoints to the same location on the map using the `way.yaml` file. It is important to note that the `way.yaml` file must be saved in the same location as the map file.

<div align="center">
     <img src="doc/wp_doc_001.png" alt="Rviz" width="650px">
</div>


**Warning** :
It needs to have the `robot_data` version with the `way.yaml` files.
