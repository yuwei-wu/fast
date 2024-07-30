# Fast-Planner 

This is the revised version on Ubuntu 20.04/ROS noetic, which can work with the controller here: https://github.com/KumarRobotics/kr_mav_control

Independent planning module, code revised from fast planner: https://github.com/HKUST-Aerial-Robotics/Fast-Planner


1. clone the repo and complie it:

```console
$ git clone -b kr git@github.com:yuwei-wu/Fast-Planner.git
$ wstool init && wstool merge Fast-Planner/fast.rosinstall && wstool update
$ cd ..
$ catkin build
```

2. run the code, you can directly copy the launch_bench.bash to the vitfly folder and run it
in one terminal, run:
```
 bash launch_bench.bash 1 vision
```

open another terminal, run:
```
roslaunch plan_manage sim.launch
```


3. navigate the drone

it will fly forward as the Vitfly. You can adjust the forward distance and goal. Let me know your desired velocity and there might be some paramters to be tuned.






