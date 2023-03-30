# gazebo_ros
For humble &amp;&amp; garden version

## 1. Clone this package in an independent folder

`mkdir -p ~/gazebo_ws/src && cd ~/gazebo_ws/src`

`git clone https://github.com/leledeyuan00/gazebo_ros.git`

## 2. Install dependencies by using rosdep

Configure your rosdep first [rosdep wiki](http://wiki.ros.org/rosdep).

`sudo rosdep init`

`rosdep update`

`cd ~/gazebo_ws`

`rosdep install --from-paths src --ignore-src -r -y`

## 3. Compile this workspace

`export GZ_VERSION=garden`

`colcon build`

## 4. Source this space to the bashrc

`echo "source ~/gazebo_ws/install/setup.bash" >> ~/.bashrc`
