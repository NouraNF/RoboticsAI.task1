# RoboticsAI.task1

## The first task of Robotics and AI department about download ROS:

### First step: 

download VirtualBox.

### Second step:

download the Ubuntu desktop.

### Third step:

create a new VM in VirtualBox.

### Forth step:

install ubuntu in vm:

1. install ubuntu in vm.
2. install ROS noetic:
```   
bash
sudo apt update
sudo apt install -y curl gnupg2 lsb-release
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
sudo apt update
sudo apt install -y ros-noetic-desktop-full
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
 ```

3. create workplace:
```
bash
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws
catkin_make
echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc
source ~/.bashrc
```   

### Fifth step:
install robot arm package:
```
bash
sudo apt install ros-noetic-robot-arm-package
```
to inatall the package replace actual package name.
