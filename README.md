# gnss_localizer
Transform the coordinate of localization got by LG simulator from LLA to ENU at NCKUEE building.

## Overview

From LG simulator, you can add a topic named "nmea_sentence" to receive the true location of the vehicle in the coordinate LLA in the simulator. 

This package subscribes `/nmea_sentence` and publishes the location of the vehicle to `/gnss_pose` in the coordinate ENU at NCKUEE building in type, geometry_msgs/PoseStamped.
