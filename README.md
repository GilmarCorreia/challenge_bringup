# challenge_bringup

ROS 2 orchestration package to launch the full capture and tracking pipeline.

The default launch runs:
- `cam_pub` or `cam_pub_threaded` to publish webcam images.
- `object_tracker` to detect the colored object and publish its state.

Main parameters:
- `threaded` (false/true): selects the standard or threaded cam_pub node.
- `color`: detection color (`yellow`, `red_lower`, `red_upper`, `orange`, `green`, `blue`).
- `param_file_path`: path to the YAML parameter file used by both nodes.
