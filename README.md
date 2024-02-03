# waiter_robot_with_stvl_navigation

This repository contains code for a waiter robot that operates using a 2D map created with GMapping, AMCL for localization, Move Base for navigation, and STVL for dynamic world perception.

## Map Creation
To create the map, follow the instructions at [link to map creation tutorial].

## Loading Map
After creating the map, load it using `map_server`.

## Starting Navigation
Initiate Move Base with STVL to begin navigation.

## Running the Workspace
1. Make a ROS workspace:
    ```bash
    mkdir -p your_name_ws/src
    ```
2. Navigate to your workspace:
    ```bash
    cd your_name_ws/src
    ```
3. Clone this repository:
    ```bash
    git clone https://github.com/Ahmed-M0ataz/waiter_robot_with_stvl_navigation.git
    ```
4. Launch robot description to spawn the robot in Gazebo and add all necessary sensors:
    ```bash
    roslaunch waiter_robot_description_pkg robot_descripion.launch
    ```
   ![Robot Description](link_to_image1)

5. Launch navigation with STVL:
    ```bash
    roslaunch waiter_robot_navigation_pkg waiter_navigation_stvl.launch
    ```
   ![Navigation with STVL](link_to_image2)
