# Installation Guide

## Automatic Installation
To use the automatic installation, you will need `curl`. If you don't have it already installed, you can install it via
```sh
sudo apt install curl
```
Once you have curl installed, start installing Arena-Rosnav by running:
```sh
curl https://raw.githubusercontent.com/Arena-Rosnav/arena-rosnav/master/install.sh | bash
```
You will be able to choose if you want to install only the essential features or the required packages for training and additional planners as well. 

### Things to note
ROS and by extension Arena-Rosnav are *big*. You should have at least 30GB of storage available.
Also, this installation will probably take about half an hour, varying depending on the speed of your internet and machine.
Arena-Rosnav is only intended to be run on Ubuntu 22.04. If you are intending to run it on a VM, be aware that you need a GPU for certain functions.

## Testing
With the activated environment, test your installation by running the command

```sh
roslaunch arena_bringup start_arena.launch simulator:=gazebo
```

This should open gazebo and rviz successfully.

# Troubleshooting
If you encounter errors during the build process due to missing packages, add them

