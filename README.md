# Safe Navigation Duckietown Project

## Description
This is a Duckietown Safe Navigation project which aims to enhance the autonomous navigation capabilities of Duckiebots within the Duckietown environment. This project focuses on improving lane following and implementing intersection navigation and obstacle avoidance to ensure safe and efficient movement of Duckiebots in a miniature city.

## Project Structure
The project is organized into several main directories:

- ***assets***: Contains various resources and configurations used by the project
- ***launchers***: Includes scripts for launching different components of the project
- ***packages***: Contains the core functionalities of the project, divided into several packages

### Packages
- ***anti_instagram***: Handles color correction
- ***apriltag***: Detects signs
- ***complete_image_pipeline***: Runs the enture image processing pipeline
- ***ground_projection***: Projects detected lane segments onto the ground plane
- ***image_processing***: Decodes, rectifies, and preprocesses images 
- ***lane_control***: Generates control commands to keep the Duckiebot within the lane
- ***lane_filter***: Estimates the Duckiebot's position and orientation within the lane
- ***led_emitter***: Controls the LED patterns on the Duckiebot
- ***led_joy_mapper***: Maps joystick inputs to LED patterns
- ***led_pattern_switch***: Switches LED patterns based on the state of the Duckiebot
- ***line_detector***: Detects lane markings
- ***nn_model***: Loads and runns the neural network model for object detection
- ***object_detection***: Classifies and filters detected objects
- ***solution***: Includes paramters for object detection
- ***stop_line_filter***: Filters and processes stop line detections
- ***utils***: Contains unitlity functions for object detection
- ***vehicle_detection***: Identifies other vehicles using the dot pattern
- ***visualization_tools***: Provides tools for visualizing various aspects of the project

## How to build and run the project on a Duckiebot:
```
dts devel build -f -H <ROBOT_NAME>
dts devel run -H <ROBOT_NAME>
```

## Additional Information
For a detailed report on the project, including the implementation of key functionalities such as lane following, intersection navigation, and object detection, please refer to the `Final_Report.pdf` file in the repository.

For a presentation overview of the project, refer to the `Final_Presentation.pptx` file in the repository.

You can access the demo video of the project [here](https://youtu.be/0AisAz7qiFU).

