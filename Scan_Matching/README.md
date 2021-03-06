# Scan Matching
The second assignment for Self-Driving Cars, 2018 Spring, NCTUEE.

## Implemantation Details
You will have two point cloud data(in .pcd format)
```
- Target
- Scene
```

You should register the scene to the target by [ICP algorithm](http://docs.pointclouds.org/trunk/classpcl_1_1_iterative_closest_point.html) and [initial alignment](http://docs.pointclouds.org/1.7.1/classpcl_1_1_sample_consensus_initial_alignment.html) for better result.

Download the .pcd data here:
- [target](https://drive.google.com/open?id=1fwtY0iXM2zbjaMjIPrWtkYzg9icNZJ8u)
- [scene](https://drive.google.com/open?id=1zM5qwsZRcAugGn-vlBmgevj6j01IF9vf)

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
You will need to do matrix operation during implementation: Use Eigen3
Note: It is already installed when installing ROS
If not, you can install Eigen3:
```
sudo apt-get install libeigen3-dev
```
- [Eigen3 Tutorial](http://eigen.tuxfamily.org/dox-devel/group__QuickRefPage.html)
- For python, see [here](https://github.com/jrl-umi3218/Eigen3ToPython)

## Running the test
How to run the automated tests for this system

### Break down into steps

`roscore`

`rosrun Scan_Matching scan_matching.cpp`

`rviz`

### Results
You should be able to see the transformation matrix in the console and also data in Rviz
```
Transformation Matrix: 

           1 -3.85962e-05  0.000732879  0.000706259
 3.96739e-05     0.999999  -0.00141144   0.00179347
-0.000732833   0.00141147     0.999999   0.00793144
           0            0            0            1
```

## Built With
- [ROS](http://www.ros.org/)
- [PCL](http://docs.pointclouds.org/trunk/index.html)
- [pcl_conversions](http://wiki.ros.org/pcl_conversions)
- [Eigen3](http://eigen.tuxfamily.org/index.php?title=Main_Page)

## Authors
- **Arthur Hsieh** - *initial work* - [arthur960304](https://github.com/arthur960304)



