# ROS-Installation
Steps to download the rose system
1-Download and install VirtualBox.<img width="220" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٥ في ١١ ١١ ٠٥ م" src="https://user-images.githubusercontent.com/108140215/178856868-dbc679ef-3741-4c47-9721-1b3f9990b45b.png">
<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٥ في ١١ ١٠ ٤٧ م" src="https://user-images.githubusercontent.com/108140215/178856887-f7c3b7b3-e802-423d-9237-4b8adb4193a2.png">
2-1-Download Ubuntu 20.04.4 LTS Desktop Image from this URL
https://releases.ubuntu.com/20.04/ubuntu-20.04.4-desktop-amd64.iso<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٥ في ١١ ١١ <img width="441" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٥ في ١١ ١١ ٢٨ م" src="https://user-images.githubusercontent.com/108140215/178857007-7f206e1c-6436-49bc-8a15-ec97e9e0935c.png">
١٧ م" src="https://user-images.githubusercontent.com/108140215/178856952-8ea4677b-9951-421a-90b1-d25aa616df8a.png">


3-click New to make a new virtual machine.<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١ ٤٦ ١٥ ص" src="https://user-images.githubusercontent.com/108140215/178857041-a88496ca-155e-4f72-a892-f6b581eef196.png">
![Uploading ‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١.٤٦.٣٩ ص.png…]()
<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١ ٤٦ ٤٩ ص" src="https://user-images.githubusercontent.com/108140215/178857054-ec8c14ac-2f14-40e2-8989-d14cefa9d118.png">
<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١ ٥١ ٠٢ ص" src="https://user-images.githubusercontent.com/108140215/178857090-a50d47e1-81fa-473d-aa52-4eb2bdf018c5.png">
![Uploading ‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١.٥٢.٠٢ ص.png…]()
![Uploading ‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١.٥٥.٠١ ص.png…]()
![Uploading ‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١.٥٥.٠٣ ص.png…]()
Note: Choose a symbol that is simple and easy to remember
<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ١ ٥٦ ٣١ ص" src="https://user-images.githubusercontent.com/108140215/178857326-0474126b-b3df-45f3-ae7f-eacf3ff8ea9b.png">
<img width="1440" alt="‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ٢ ٠٢ ٤٨ ص" src="https://user-images.githubusercontent.com/108140215/178857325-f3327eb1-97cc-422a-9c5a-d39fe823bb1a.png">
![Uploading ‏لقطة الشاشة ١٤٤٣-١٢-٠٦ في ٢.٠٦.١٧ ص.png…]()

Enter the commands from this site "s-m.com.sa/ros.txt"


These are all the commands you need to install the system



sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

sudo apt-get update

sudo apt-get install ros-kinetic-desktop-full

apt-cache search ros-kinetic

echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc

sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

sudo apt install python-rosdep

sudo rosdep init

rosdep update

sudo apt-get install ros-noetic-catkin

mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-kinetic-moveit

sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line
(source /home/wesam/catkin_ws/devel/setup.bash)
then 
ctrl + o

source ~/.bashrc


roslaunch robot_arm_pkg check_motors.launch

These are all the commands you need to install the system
Reference:
https://youtu.be/fr6TXEd2rXI
https://www.youtube.com/watch?v=vfqN-RRt84Q&pp=ugMICgJhchABGAE%3D
https://www.youtube.com/watch?v=P9UCYSWv3Ho&pp=ugMICgJhchABGAE%3D
