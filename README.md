# DiffDrive_ws-ROS2

A ROS2 workspace implementing a full software stack for a differential-drive mobile robot ("bumperbot"), covering everything from low-level firmware to navigation and mapping.

## 📦 Packages

| Package | Purpose |
|---|---|
| `bumperbot_description` | Robot URDF/model description |
| `bumperbot_firmware` | Low-level hardware interface |
| `bumperbot_bringup` | Launch files to start the robot stack |
| `bumperbot_controller` | Differential drive controller |
| `bumperbot_motion` | Motion control logic |
| `bumperbot_localization` | Robot localization (e.g. odometry/sensor fusion) |
| `bumperbot_mapping` | Mapping (SLAM) |
| `bumperbot_navigation` | Autonomous navigation (Nav2) |
| `bumperbot_planning` | Path/motion planning |
| `bumperbot_msgs` | Custom ROS2 message/interface definitions |
| `bumperbot_utils` | Shared utility code |
| `bumperbot_py_examples` | Python example nodes |

## 🛠️ Tech

- **Framework:** ROS2
- **Language:** Python (with URDF/XML for description)
- Includes generated TF frame trees (`frames_*.pdf`) for debugging the robot's transform hierarchy

## 🚀 Usage

```bash
# From the workspace root
colcon build
source install/setup.bash
ros2 launch bumperbot_bringup <launch_file>.launch.py
```

(Adjust the launch file name based on whether you're running in simulation or on real hardware.)

## 📌 Notes

This workspace was built while learning ROS2 fundamentals — differential drive kinematics, localization, mapping, and Nav2-based navigation.
