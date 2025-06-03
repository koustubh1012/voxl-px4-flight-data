# 🛰️ voxl-px4-flight-data

This repository provides access to a collection of **ROS bag files** containing synchronized **camera imagery** and **vehicle odometry** data, intended to support robotics research and development. The datasets are hosted on Google Drive for public access.

![GIF](/dataset.gif)

## 📁 Dataset Contents

Each ROS bag file includes:

- **Image Data**: Captured from forward-facing camera. Stored under topics such as `/small_hires_color`.
- **Odometry Data**: ROS messages of type `nav_msgs/Odometry` or `px4_msgs/VehicleOdometry` representing the vehicle's position, orientation, and velocity.
- **Timestamp Synchronization**: All topics are time-aligned, enabling accurate data playback and processing.

These datasets are well-suited for applications such as:
- SLAM and visual odometry
- Sensor fusion and state estimation
- Path planning and trajectory analysis
- Perception system evaluation
- 3D reconstruction

---

## 🔗 Download Links

The datasets are available via Google Drive. Click the link below to download:

https://drive.google.com/drive/folders/1pg_ahzVkooheTqEthO22IWTJKCMvQ9rM?usp=drive_link

| Dataset Name                    | Description                                               
|---------------------------------|----------------------------------------------------------------|
| `traffic_cone`                  | Indoor footage of drone circling around a traffic cone         |
| `fearless_flight_facility`      | Outdoor drone footage with manequins and fire pits             |
| `gps`                           | Comparison between gps based outdoor localization and qvio     |
| `april_tag`                     | Indoor drone footage of tracking camera and vehicle odometry   |
|                                 | while tracking and following an april tag                      |

> ⚠️ Ensure you are signed into a Google account to access the files. If you encounter permission issues, please open a GitHub issue or email me.

---

## Dependencies

[px4_msgs](https://github.com/PX4/px4_msgs.git) v1.14 

## 🚀 Quick Start

### ROS 2
To play a `.bag` file:
```bash
ros2 bag play <file_name>
```

## 📚 Citation

If you use this dataset in your research, please cite this repository:
```bibtex
@misc{ros_bag_dataset,
  author       = {FNU Koustubh, Keyur Borad},
  title        = {ROS Bag Dataset for UAV Research},
  year         = {2025},
  howpublished = {\url{https://github.com/koustubh1012/voxl-px4-flight-data.git}},
  note         = {Accessed: 2025-06-02}
}
```

## 📬 Contact

For questions, access requests, or collaboration inquiries, contact:

Koustubh – koustubh1012@gmail.com
