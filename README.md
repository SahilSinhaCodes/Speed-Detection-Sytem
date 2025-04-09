# Speed Estimation Using YOLOv8

## Overview
This repository implements a vehicle speed estimation system using the YOLOv8 object detection model and a custom tracking algorithm. The program processes video footage to detect vehicles, track their movement, and estimate their speed as they cross predefined lines.

## Features
- Vehicle detection using YOLOv8.
- Custom tracking algorithm for assigning unique IDs to vehicles.
- Speed estimation based on time taken to cross two horizontal lines.
- Saves annotated frames and generates an output video.

## Requirements
Install the required Python packages:
pip install ultralytics opencv-python pandas


## Usage
1. Clone the repository:
git clone (https://github.com/SahilSinhaCodes/Speed-Detection-Sytem)



2. Place your input video file (e.g., `highway.mp4`) in the root directory.

3. Run the script:
python speed_estimate.ipynb


4. Output:
- Annotated frames are saved in the `detected_frames` folder.
- Final annotated video is saved as `output.avi`.

## Configuration
- Adjust `red_line_y` and `blue_line_y` in the script to set line positions for speed estimation.
- Set `distance` (default: 10 meters) to match real-world distance between the two lines.

## Output Example
The output includes:
- Bounding boxes around detected vehicles.
- Vehicle IDs and speeds displayed near bounding boxes.

## Notes
- Ensure your input video resolution matches or is resized appropriately for optimal performance.
- Accuracy depends on correct calibration of real-world distances.

## Acknowledgments
This project uses:
- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) for object detection.
- OpenCV for image processing and visualization.
