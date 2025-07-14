# 🎯 Red Object

A Python project that detects and tracks red-colored objects in a video using the OpenCV library.  
The script reads a video file, identifies red regions using color segmentation in the HSV space, draws bounding boxes, and exports the final output as a GIF.

---

## 📁 Project Files

- `7237152-sd_360_640_25fps.mp4` : Original input video used for processing.
- `color.py` : Python script for red color detection and processing.
- `output.gif` : Output GIF showing the red object tracking result.

---

## 🧰 Requirements

- Python 3.x (recommended with Anaconda)
- OpenCV
- imageio

Install the required libraries using:

```bash
pip install opencv-python imageio
▶️ How to Run
Make sure all project files are in the same folder.

Run the Python script:

bash
نسخ
تحرير
python color.py
A window will appear showing the processed video with red object tracking, and a GIF will be saved as output.gif.

💡 How It Works
The script converts each frame to HSV color space.

It applies a color mask to detect red tones using two ranges:

Lower red (0–10 hue)

Upper red (170–180 hue)

Morphological operations (opening and dilation) are applied to remove noise.

Contours are found and drawn as green rectangles over red areas.

Each frame is collected and exported as a GIF.

📷 Output Preview
🎥 Original Video:
Included in the project (3765188-uhd_3840_2160_30fps.mp4)

🧪 Processed Output:

🪪 License
This project is open-source and free to use for educational and experimental purpose
