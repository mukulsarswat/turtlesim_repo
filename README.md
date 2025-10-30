
# 🐢 Turtlesim Cleaner

A ROS-based simulation project that demonstrates autonomous cleaning strategies using the Turtlesim environment. This repository  showcases multiple motion planning techniques for full-area coverage—similar to robotic vacuum cleaners.

>  **Note:**  Implementation based on [YouTube tutorials](https://www.youtube.com/playlist?list=PLSzYQGCXRW1HLWHdJ7ehZPA-nn7R9UKPa).

---

## 📦 Project Structure

This package contains five C++ implementations, each demonstrating a unique cleaning strategy:

| File | Description |
|------|-------------|
| `robot_cleaner_move_rotate.cpp` | Basic movement and rotation logic |
| `robot_cleaner_abs_orientation.cpp` | Absolute orientation control |

---

## 🚀 Getting Started

### 1. Create the Package

```bash
cd ~/catkin_ws/src
catkin_create_pkg turtlesim_cleaner
cd ~/catkin_ws
catkin_make
```

### 2. Add Source Files

```bash
cd ~/catkin_ws/src/turtlesim_cleaner
mkdir src
# Add desired .cpp file from this repo into src/
```

Replace your `CMakeLists.txt` and `package.xml` with the ones provided in this repository.

---

## 🧪 Run the Demo

```bash
roscore                            # Start ROS Master
rosrun turtlesim turtlesim_node   # Launch Turtlesim
rosrun turtlesim_cleaner robot_cleaner_node  # Run your selected cleaner
```

---

## 📚 Resources

- 🐢 [Turtlesim Wiki](http://wiki.ros.org/turtlesim)
