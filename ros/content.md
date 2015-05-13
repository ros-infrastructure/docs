# What is [ROS][@ROS.org]?

The Robot Operating System (ROS) is a set of software libraries and tools that help you build robot applications. From drivers to state-of-the-art algorithms, and with powerful developer tools, ROS has what you need for your next robotics project. And it's all open source.

> [wikipedia.org/wiki/Robot_Operating_System](https://en.wikipedia.org/wiki/Robot_Operating_System)

[%%LOGO%%][@ROS.org]

# How to use this image

## Create a `Dockerfile` in your ROS app project

    FROM ros:indigo
    # place here your application's setup specifics
    CMD [ "roslaunch", "my-ros-app my-ros-app.launch" ]

You can then build and run the Docker image:

    docker build -t my-ros-app .
    docker run -it --rm --name my-running-app my-ros-app

# More Resources

[ROS.org][@ROS.org]: Main ROS website  
[Wiki][@ROS_Wiki]: Find tutorials and learn more  
[ROS Answers][@ROS_Answers]: Ask questions. Get answers  
[Blog][@ROS_Blog]: Stay up-to-date  
[OSRF][@OSRF]: Open Source Robotics Foundation  

[@ROS.org]:     http://www.ros.org/ "Main ROS website"
[@ROS_Wiki]:    http://wiki.ros.org/ "Find tutorials and learn more"
[@ROS_Answers]: http://answers.ros.org/questions/ "Ask questions. Get answers"
[@ROS_Blog]:    http://www.ros.org/news/ "Stay up-to-date"
[@OSRF]:        http://www.osrfoundation.org/ "Open Source Robotics Foundation"

[@ROS_Logo]:    https://raw.githubusercontent.com/docker-library/docs/master/ros/logo.png "ROS Logo"
