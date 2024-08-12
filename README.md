# Self-balancing-robot
Self-balancing robot with pid controller and arduino

# Note
if you want use the code make sure to set new offset and pid values

# 3d design
The design have done using SolidWorks.<br/>
you can check the design in 3d design folder

# Hardware
  the project run on arduino uno with mpu6050 gyroscope.<br/>
  the sensor read the value of the angle and the motors go forward and backward.<br/>
  to let the robot stand based on pid controller

# Software
the code written in c++ language.<br/>
libraries:<br/>
PID_v1.h <br/>
I2Cdev.h<br/>
MPU6050_6Axis_MotionApps20.h

# The Control Theory
The control algorithm used in this project is PID Control algorithm which provides pretty decent results.<br/>
For tuning the controller constants we mainly focused on the plotting and creat a track bar window to choose the values for the constants Kp,Ki,Kd.<br/>
This method makes it easier to tune the PID parameters in real-time and visualize the graph in plotting window.<br/>

At first make all of Kp,Ki,Kd zero then start tuning the Proportional term which will make an overshoot in the system, then tuning Derivative term which will reduce the over shoot of the system to make it much more reasonable, finaly the system will have a steady state error and by tuning the Integral term it will be so close to zero.<br/>

# Youtube video

# resources
pid controller:<br/>
https://www.ni.com/en/shop/labview/pid-theory-explained.html?srsltid=AfmBOoq3-fylmllxyo6L2iQQYDV7p2_QuoJby15Ih8ZvtyOjQv_LiGNj<br/>
self-balancing studying:<br/>
https://www.researchgate.net/publication/327015585_Designing_an_Object_Tracker_Self-Balancing_Robot
