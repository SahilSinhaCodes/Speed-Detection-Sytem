# 🚗 Vehicle Speed Estimation using YOLOv8 and OpenCV

This project estimates the speed of vehicles in a video using object detection (YOLOv8), tracking, and OpenCV. It assigns IDs to each vehicle and calculates their speeds based on movement across frames.

---

## 📁 Project Structure

├── main.py # Main script to run vehicle speed estimation
├── tracker.py # Tracking logic for assigning IDs to vehicles
├── vehicles.mp4 # Sample video footage (input)
├── README.md # Project documentation

yaml
Copy
Edit

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/vehicle-speed-estimation.git
cd vehicle-speed-estimation
2. Install Dependencies
Make sure you have Python 3.8+ and pip installed.

bash
Copy
Edit
pip install ultralytics opencv-python
3. Add a Video
Place your video file in the root directory and rename it to:

Copy
Edit
vehicles.mp4
Alternatively, update the filename in main.py if you want to use a different name.

🧠 How It Works
YOLOv8 detects vehicles frame-by-frame.

A custom tracker (from tracker.py) assigns unique IDs to each vehicle.

Speeds are estimated by measuring pixel distance moved across frames and converting it using a scaling factor (based on assumptions).

🛠️ Configuration Notes
The current speed calculation assumes a fixed scale — for accurate real-world speed, you’d need to calibrate based on camera angle and scene depth.

Detected speeds are overlaid in km/h on the video output.

▶️ Run the Project
bash
Copy
Edit
python main.py
This will open a window showing vehicles with bounding boxes, unique IDs, and estimated speeds.

📦 Requirements
Python 3.8+

OpenCV

Ultralytics (for YOLOv8)

Install them using:

bash
Copy
Edit
pip install opencv-python ultralytics
📸 Sample Output
Bounding boxes with vehicle IDs

Speed in km/h displayed above each vehicle

📄 License
This project is licensed under the MIT License.

✨ Credits
YOLOv8 by Ultralytics

Inspired by real-time object tracking use-cases and traffic analytics
