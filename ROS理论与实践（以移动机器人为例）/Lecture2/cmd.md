roscore
启动ROS服务

rosrun turtlesim turtlesim_node
启动海龟节点

rosrun turtlesim turtle_teleop_key 
启动键盘控制

rosservice call /spawn 
输入后按tab键，得到

rosservice call /spawn "x: 0.0
y: 0.0
theta: 0.0
name: 't1'" 
回车生成新的名叫t1的海龟

rosservice call /spawn "x: 0.0
y: 0.0
theta: 0.0
name: 't2'" 
生成t2海龟

rostopic pub /t1/cmd_vel geometry_msgs/Twist
使用tab键，得到

rostopic pub /t1/cmd_vel geometry_msgs/Twist "linear:
  x: 0.0
  y: 0.0
  z: 0.0
angular:
  x: 0.0
  y: 0.0
  z: 0.0
  z: 0.0
angular:
  x: 0.0
  y: 0.0
  z: 0.0"
修改后回车可观察到海龟位置变化



