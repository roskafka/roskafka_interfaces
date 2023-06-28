# roskafka_interfaces

roskafka_interfaces is a ROS (Robot Operating System) 2 package that provides interface specifications for the [roskafka](https://gitlab.informatik.hs-furtwangen.de/ss23-forschungsprojekt-7/roskafka) ROS 2 package.

## Setup

Download code to ROS 2 workspace:

    mkdir -p ~/ros2_ws/src
    cd ~/ros2_ws/src
    git clone https://gitlab.informatik.hs-furtwangen.de/ss23-forschungsprojekt-7/roskafka_interfaces.git

Build package:

    cd ~/ros2_ws
    PYTHONWARNINGS=ignore:::setuptools.command.install colcon build --packages-select roskafka_interfaces

Source package:

    . install/setup.bash

Verify that service interfaces exist:

    ros2 interface show roskafka_interfaces/srv/AddMapping
    ros2 interface show roskafka_interfaces/srv/RemoveMapping
