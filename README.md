# Manipulate Turtlesim On ROS NOETIC
this project provide a guide to running TurtleSim package on ROS Noetic with instruction to control turtle movement using keyborad 

## REQUIREMENTS :
- UBUNTU 20.04
- ROS NOETIC 
- Installing turtlesim package

---
## INSTALLIATION :
```
sudo apt update 
sudo apt install ros-noetic-turtlesim
```
---
## OPEN ROS SYSTEM :
- Open three terninal
- start by write ' roscore ' to start rosmaster
```
roscore
rosrun turtlesim turtlesim_node
```

![1](https://github.com/user-attachments/assets/5255df65-a47f-4d90-9014-742b394310a6)

---
## SHOW ACTIVE NODES 
In a new terminal I wrote rosnode list to show all active nodes 
```
rosnode list
```
## SHOW ACTIVE TOPICS 
In a new terminal I wrote rosnode list to show all active topics 
```
rostopic list
```
---

## EXPLORE FUNCTIONALITIES 
In a new terminal I wrote this command to make the turtle move in square :

```
rosrun turtlesim draw_square 
```
![photo_2024-07-18_04-52-43](https://github.com/user-attachments/assets/d0a65dc3-1d5c-4a7a-9a1b-2e8350785206)

and I wrote this command in another terminal to see changes in poses of the turtle 

```
rostopic echo /turtle1/pose 
```
---
## NODE INFORMATION 
In another terminal I wrote this command to know information about node 
```
rosnode info /turtlesim  
```
---
## MOVING THE TURTLE :
In another terminal I wrote this command to move turtle by arrow keys 

```
rosrun turtlesim turtle_teleop_key 
```


![last thing](https://github.com/user-attachments/assets/02785f2b-5101-402c-b51b-c5a068849721)


