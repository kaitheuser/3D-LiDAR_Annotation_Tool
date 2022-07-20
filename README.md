# 3D LiDAR Annotation Tool with pcd2bin Conversion Tool
## git clone from songanz/3D-LiDAR-annotator
UCSD Autonomous Vehicle Laboratory (AVL) 3D-LiDAR Annotation Tool

# Citation
``` 
   @article{wang2019latte,
      title={LATTE: Accelerating LiDAR Point Cloud Annotation via Sensor Fusion, One-Click Annotation, and Tracking},
      author={Wang, Bernie and Wu, Virginia and Wu, Bichen and Keutzer, Kurt},
      journal={arXiv preprint arXiv:1904.09085},
      year={2019}
   }
   ```

# OS and App Requirements
0. Ubuntu 16.04 LTS
1. Python 3.7.13
2. ROS Kinetic
3. Google Chrome

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

# Installation
0. Git clone the repository
    * `git clone https://github.com/kaitheuser/3D-LiDAR_Annotation_Tool.git`
1. Change directory to `3D-LiDAR_Annotation_Tool` folder
    * `cd 3D-LiDAR_Annotation_Tool`
2. Install dependencies
    * `pip3 install -r requirements.txt`

# How to Run the 3D LiDAR Annotation Tool with pcd2bin Conversion Tool Application
0. Change directory to `3D-LiDAR_Annotation_Tool` folder
    * `cd 3D-LiDAR_Annotation_Tool`
1. Navigate to the `app` folder in the `3D-LiDAR_Annotation_Tool` folder
    * `cd app`
2. Run the `app.py` to launch the application.
    * `python3 app.py`
3. Decide whether to convert the pcd files to bin files.
    * `Y` -> Choose to convert
    0.  Browse For PCD File Directory
    1.  Choose a Directory to save the .bin files
    2.  Click the **Convert PCD to BIN** button to convert
    * `N` -> Already converted
4.  Open **http://127.0.0.1:5000** on the Chrome Browser

# How to Annotate 3D-LiDAR Point Clouds or Objects
0. 







        
