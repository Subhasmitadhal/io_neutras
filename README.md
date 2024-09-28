# io_neutras
# UAV Applications
This project aims to provide an advanced solution for disaster management and climate monitoring using unmanned aerial vehicles (UAVs). The system is designed to help authorities monitor affected areas in real time, map terrains, and respond effectively to natural disasters such as floods, earthquakes, and wildfires.

# Pulsar UAV Project

## Project Overview
The Pulsar UAV project leverages advanced drone technology to enhance applications in areas such as disaster management, industrial inspections, environmental monitoring, and agricultural assessments. Designed for versatility and high performance, the Pulsar UAV is equipped with state-of-the-art sensors and navigation systems.

## Key Technologies
- High-Resolution Imaging
- Thermal Imaging
- LiDAR
- Autonomous Navigation
- AI Integration
 
## Features
- Real-time data transmission and monitoring
- Modular payload system for various sensor configurations
- Intelligent flight planning and autonomous operation capabilities
- User-friendly ground control interface
- High endurance for extended mission durations

## Hardware Components
- UAV Platform
- Cameras
- LiDAR Unit
- Ground Control Station
- Communication System

##Software Setup


-*Ros2 installation* 
```bash
first install Ros 2
sudo apt update && sudo apt upgrade -y
sudo locale-gen en_US en_US.UTF-8
sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
export LANG=en_US.UTF-8
sudo apt install software-properties-common
sudo add-apt-repository universe
sudo apt update && sudo apt install curl gnupg lsb-release
sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
sudo sh -c 'echo "deb [arch=arm64] http://packages.ros.org/ros2/ubuntu $(lsb_release -cs) main" > /etc/apt/sources.list.d/ros2-latest.list'
sudo apt update
sudo apt install ros-foxy-desktop
sudo apt install python3-colcon-common-extensions python3-rosdep2 python3-vcstool git
echo "source /opt/ros/foxy/setup.bash" >> ~/.bashrc
source ~/.bashrc
sudo rosdep init
rosdep update
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws/
colcon build
source ~/ros2_ws/install/setup.bash
echo "source ~/ros2_ws/install/setup.bash" >> ~/.bashrc





-*SLAM installation*

Install SLAM In Ros2 Env
ros2 pkg list | grep slam_toolbox
sudo apt install ros-foxy-navigation2
sudo apt install ros-foxy-nav2-bringup
sudo apt install ros-foxy-map-server ros-foxy-amcl ros-foxy-lifecycle-msgs
sudo apt install ros-foxy-turtlebot3 ros-foxy-turtlebot3-simulations
export TURTLEBOT3_MODEL=burger
ros2 launch turtlebot3_cartographer cartographer.launch.py
ros2 launch slam_toolbox online_async_launch.py
ros2 launch nav2_bringup rviz_launch.py
```
Our innovation is 

Swarm technology in drones refers to the coordination and control of multiple drones (or UAVs) to work together as a unified system to achieve common goals. which operate using decentralized control and self-organization principles.
The drones in a swarm need to communicate with each other. This can be done through wireless protocols or specialized communication protocols tailored for drone-to-drone communication. MAVLink is commonly used in UAV communication.

Creat a python virtual environment
```bash
# sudo apt install python3
# sudo apt install python3-pip
# python3 -m venv myenv
# source myenv/bin/activate
```
```bash
# install torch
# install csv
# install argpars
```



