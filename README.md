# Autonomous-ATV-IIT-Kharagpur
Autonomous Ground Vehicle Laboratory(AGV lab) , IIT Kharagpur

Keywords: ROS,Autonomous-vehicles,3D-mapping

This project was done during the summer of 2017 at AGV lab, IIT Kharagpur under the guidance of Dr. Debashish Chakraborty. The main aim of the project was to lay the ground work for developing an autonomous delivery robot. ROS was used with Ubuntu 16.04 as master while raspbian was used on raspberry pi and ROS slave. Using roskinetic api with added features of rosbridge to google map API and mavros link to Arducopter's database , an autonomous all terrain vehicle was made. The Arducopter APM2.8 was used as a sensor hub as it incorporates IMU, GPS, Barometer data all together so that we do not require interfacing all the sensors individually.An attempt to make a 2D plot using a Lidar was successful.

Hardware Used :
Raspberry 3 (Raspbian OS)
ATMEGA2560
APM2.8
GPS
IMU
Cytron 16Amp Dual channel motor drivers
6WD all terrain robot base

<p align="center">
  <img width="300" height="300" src="media/image004.jpg">
</p>



The above image shows our setup of the ATV designed. A kinect was later on added to the setup as an effort to obtain and integrate raw images and point clouds.

<p align="center">
  <img width="450" height="300" src="media/image002.jpg">
</p>



GUI of OpenStreetMap(osm) Application for Start and Destination points showing the current and intended positions respectively.  (The dotted line represents the path followed by robot)


<p align="center">
  <img width="580" height="300" src="media/image002%20(1).jpg">
</p>

rqt graph of all active nodes and topics for executing the robot movements in this study


<p align="center">
  <img width="600" height="300" src="media/Screenshot%20from%202018-05-28%2011-48-58.png">
</p>


3D scatter plotting of distant obstacles.

This ATV has only been tested on roads for waypoint navigation using google roads api. The future work of this project would be to integrate it with an appropriate method of slam so that it can render the the complete surroundings so that it can be more aware of its surroundings. 
