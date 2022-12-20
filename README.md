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
## Adding and Editing Waypoints
To add waypoints, click on the Waypoint Navigation Tool in the Rviz toolbar, and then click on the Rviz scene to place a waypoint. You can add multiple waypoints by repeating this process.

To update the location of a waypoint, you can either drag the interactive marker associated with the waypoint, or use the Rviz panel to specify the new position.

<div align="center">
     <img src="doc/wp_doc_002.png" alt="Rviz" width="650px">
</div>

## Save Waypoints

Para salvar os waypoints que foram adicionados no Rviz, primeiro clique no waypoint desejado na ferramenta Rviz. Em seguida, salve os pontos de referência no mesmo local do mapa usando o arquivo `way.yaml`. É importante observar que o arquivo `way.yaml` deve ser salvo no mesmo local que o arquivo de mapa.

<div align="center">
     <img src="doc/wp_doc_001.png" alt="Rviz" width="650px">
</div>
