# Supported tags and respective `Dockerfile` links

- [`indigo-ros-base`, `latest` (*indigo/ros_base/Dockerfile*)](https://github.com/ros-infrastructure/docker_images/tree/master/indigo/ros_base/Dockerfile)
- [`indigo-ros-core`, (*indigo/ros_core/Dockerfile*)](https://github.com/ros-infrastructure/docker_images/tree/master/indigo/ros_core/Dockerfile)
- [`indigo-robot`, (*indigo/robot/Dockerfile*)](https://github.com/ros-infrastructure/docker_images/tree/master/indigo/robot/Dockerfile)
- [`indigo-perception`, (*indigo/perception/Dockerfile*)](https://github.com/ros-infrastructure/docker_images/tree/master/indigo/perception/Dockerfile)


For more information about this image and its history, please see the [relevant manifest file (`library/ros`)][@Library_ros] in the [`docker-library/official-images` GitHub repo][@Official_images].

[@Library_ros]: https://github.com/docker-library/official-images/blob/master/library/ros
[@Official_images]: https://github.com/docker-library/official-images

# What is [ROS][@ROS.org]?

The Robot Operating System (ROS) is a set of software libraries and tools that help you build robot applications. From drivers to state-of-the-art algorithms, and with powerful developer tools, ROS has what you need for your next robotics project. And it's all open source.

> [wikipedia.org/wiki/Robot_Operating_System](https://en.wikipedia.org/wiki/Robot_Operating_System)

[![logo][@ROS_Logo]][@ROS.org]

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

# License

The core of ROS is licensed under the standard three-clause BSD license. This is a very permissive open license that allows for reuse in commercial and closed source products. You can find more about the BSD license from the Opensource.org [BSD 3-Clause][@BSD_3] page and Wikipedia's [BSD Licenses][@BSD_wiki] entry.

While the core parts of ROS are licensed under the BSD license, other licenses are commonly used in the community packages, such as the [Apache 2.0][@Apache_2.0] license, the [GPL][@GPL] license, the [MIT][@MIT] license, and even proprietary licenses. Each package in the ROS ecosystem is required to specify a license, so that it is easy for you to quickly identify if a package will meet your licensing needs.

[@BSD_wiki]:    http://en.wikipedia.org/wiki/BSD_licenses
[@BSD_3]:       http://opensource.org/licenses/BSD-3-Clause
[@Apache_2.0]:  http://opensource.org/licenses/Apache-2.0
[@GPL]:         http://opensource.org/licenses/gpl-license
[@MIT]:         http://opensource.org/licenses/MIT


# Supported Docker versions

This image is officially supported on Docker version 1.4.1.

Support for older versions (down to 1.0) is provided on a best-effort basis.

# User Feedback

## Issues

If you have any problems with or questions about this image, please contact us through a [GitHub issue][@GitHub_issues].

You can also reach many of the official image maintainers via the `#docker-library` IRC channel on [Freenode][@Freenode].

## Contributing

You are invited to contribute new features, fixes, or updates, large or small; we are always thrilled to receive pull requests, and do our best to process them as fast as we can.

Before you start to code, we recommend discussing your plans through a [GitHub issue][@GitHub_issues], especially for more ambitious contributions. This gives other contributors a chance to point you in the right direction, give you feedback on your design, and help you find out if someone else is working on the same thing.

[@GitHub_issues]: https://github.com/ros-infrastructure/docker_images/issues
[@Freenode]: https://freenode.net
