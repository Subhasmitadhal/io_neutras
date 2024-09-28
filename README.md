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

