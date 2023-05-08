# robothijauump
Tutorial for Robot Hijau UMP Perception


# RobotDescriptionAizzat
Description for Robot Hijau

`roslaunch robot_description aizzat_mobile_manipulator_nolidar.launch`

`roslaunch robot_description aizzat_mobile_manipulator_2dlidar.launch`

`roslaunch robot_description aizzat_mobile_manipulator_3dlidar.launch`



## To move robot: 

`rostopic pub -r 10 /robot_base_velocity_controller/cmd_vel geometry_msgs/Twist  '{linear:  {x: 0.3, y: 0.0, z: 0.0}, angular: {x: 0.0,y: 0.0,z: 0.0}}'`

## Run using teleop

```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=/robot_base_velocity_controller/cmd_vel
```

And you can control it by typing this: 
```
Reading from the keyboard  and Publishing to Twist!
---------------------------
Moving around:
   u    i    o
   j    k    l
   m    ,    .

```




