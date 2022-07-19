# 3D LiDAR Annotation Tool with pcd2bin Conversion Tool
## git clone from songanz/3D-LiDAR-annotator
UCSD Autonomous Vehicle Laboratory (AVL) 3D-LiDAR Annotation Tool

# OS and App Requirements
0. Ubuntu 16.04 LTS
1. Python 3.7.13
2. ROS Kinetic

# Pre-requisites
0. Skip the step (Pre-requisite Step #1) below if the LiDAR data are stored in a binary float matrix format (.bin extension)
    * Each column is a point, where the rows are in the following order: 
        > x, y, z, intensity
1. Converted the bag file to pcd files. 

    ![](./gif/bag2pcd.gif)

    * Run the command below in a Linux terminal:
        
        `roscore`

    * Run the following command in a **NEW** Linux terminal:
        
        `rosrun pcl_ros bag_to_pcd <input_file.bag> <topic> <output_directory>`

        
