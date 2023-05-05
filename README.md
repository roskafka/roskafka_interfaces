# roskafka_interfaces

Initial setup:

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
