## Repository Structure


- **publisher_package**: Contains the C++ implementation of the Publisher.

- **publisher_package_py**: Contains the Python implementation of the Publisher.


## Running the Examples

### Python Version

1. **Run the Python Publisher and Subscriber**:
   - Ensure that both `publisher_package_py` and `subscriber_package_py` are located at the same directory level as `publisher_package` and `subscriber_package`.
   - Execute the Publisher:
     ```bash
     python3 ./devel/lib/publisher_package_py/publisher_code.py
     ```
   - Execute the Subscriber:
     ```bash
     python3 ./devel/lib/subscriber_package_py/subscriber_code.py
     ```

### C++ Version

1. **Build the C++ Packages**:
   - Navigate to your catkin workspace:
     ```bash
     cd ~/catkin_ws
     ```
   - Build the workspace:
     ```bash
     catkin_make
     ```

2. **Run the C++ Publisher and Subscriber**:
   - Ensure that `publisher_package` and `subscriber_package` are located at the same directory level.
   - Start the ROS core:
     ```bash
     roscore &
     ```
   - Run the Publisher:
     ```bash
     rosrun publisher_package publisher_node
     ```
   - Run the Subscriber:
     ```bash
     rosrun subscriber_package subscriber_node
     ```

## Notes

- This repository's structure is designed for the ease of assignment submission. Ensure that the packages (both C++ and Python versions) are maintained at the same hierarchical level in your workspace to avoid any runtime issues.
- Make sure you have installed all necessary dependencies and your ROS environment is correctly sourced before running the examples.
