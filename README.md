# roskafka_interfaces

roskafka_interfaces is a ROS (Robot Operating System) 2 package that provides interface specifications for the [roskafka](https://gitlab.informatik.hs-furtwangen.de/ss23-forschungsprojekt-7/roskafka) ROS 2 package.

## Setup

1. Download code to ROS 2 workspace:

        mkdir -p ~/ros2_ws/src
        cd ~/ros2_ws/src
        git clone https://gitlab.informatik.hs-furtwangen.de/ss23-forschungsprojekt-7/roskafka_interfaces.git

2. Build package:

        cd ~/ros2_ws
        PYTHONWARNINGS=ignore:::setuptools.command.install colcon build --packages-select roskafka_interfaces

3. Open a new terminal: Always source a workspace from a different terminal than the one you used `colcon build`.

4. Source ROS 2:

        source /opt/ros/humble/setup.bash

5. Source package:

        . install/setup.bash

6. Verify that service interfaces exist:

        ros2 interface show roskafka_interfaces/srv/AddMapping
        ros2 interface show roskafka_interfaces/srv/RemoveMapping
