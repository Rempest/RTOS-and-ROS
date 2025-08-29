# ROS 2 + FreeRTOS Control Loop Example

This project demonstrates how to integrate **ROS 2 (Humble)** with **FreeRTOS** in a simple control loop node.  
The node shows how real-time tasks can run alongside ROS 2 publishers, subscribers, and hardware interfaces.

___

# Features
- Uses **ROS 2 rclcpp** for creating a control node.  
- Integrates **FreeRTOS tasks** inside a ROS 2 node.  
- Example of creating:
  - Hardware interface  
  - Motor interface  
  - Subscribers  
  - Timer  
  - Publishers  

___
# Dependencies
- ROS 2 Humble (or later)  
- FreeRTOS  
- C++17 compiler  
- `colcon` build system  

___

# How it works
1. The node `ControlLoop` is created using ROS 2.  
2. Inside `control_loop()`, a **FreeRTOS task** (`MyTask`) is started, which prints `"RTOS is running"` every second.  
3. ROS 2 functions are called to simulate:
   - Hardware interface initialization  
   - Motor interface setup  
   - Creation of subscribers, publishers, and timers  

___
