This is a WIP thing.

1. Install ROS2 dashing, see [here](https://index.ros.org//doc/ros2/Installation/Dashing/Linux-Install-Debians/)
2. Install colcon, `sudo apt install python3-colcon-common-extensions`
3. Install gazebo, `curl -sSL http://get.gazebosim.org | sh`
3. Create workspace

   `cd ~`
   
   `mkdir ros2_biped`
   
   `cd ros2_biped`
   
4. Clone this repository into ~/ros2_biped/src `git clone --recursive https://github.com/pohzhiee/ros2_biped_robot.git src`
5. Run `colcon build` inside ~/ros2_biped 
6. Add relevant stuff to environment variables
`source ~/ros2_biped/install/setup.bash`
7. Add the sourcing code to .bashrc
`nano ~/.bashrc`
Add the following to the end, add your username here:
`source /home/<your_username>/ros2_biped/install/setup.bash`
8. Open new terminal

`cd ~/ros2_biped`

`colcon build`
