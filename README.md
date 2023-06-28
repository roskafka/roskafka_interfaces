# roskafka_interfaces

roskafka_interfaces is a ROS (Robot Operating System) 2 package that provides interface specifications for the [roskafka](https://gitlab.informatik.hs-furtwangen.de/ss23-forschungsprojekt-7/roskafka) ROS 2 package.

## Setup

1. Source ROS 2:

        source /opt/ros/humble/setup.bash

2. Download code to ROS 2 workspace:

        mkdir -p ~/ros2_ws/src
        cd ~/ros2_ws/src
        git clone https://gitlab.informatik.hs-furtwangen.de/ss23-forschungsprojekt-7/roskafka_interfaces.git

3. Build package:

        cd ~/ros2_ws
        PYTHONWARNINGS=ignore:::setuptools.command.install colcon build --packages-select roskafka_interfaces

## Usage

1. Open a new terminal: Always source a workspace from a different terminal than the one you used `colcon build`.

2. Source ROS 2:

        source /opt/ros/humble/setup.bash

3. Source workspace:

        source ~/ros2_ws/install/setup.bash

4. Verify that service interfaces exist:

        ros2 interface show roskafka_interfaces/srv/AddMapping
        ros2 interface show roskafka_interfaces/srv/RemoveMapping
