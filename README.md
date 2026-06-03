# 🎯 Real-Time Moving Object Detection using OpenCV

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

A real-time **moving object detection** system using Python and OpenCV. The application captures a live webcam feed, detects any motion by comparing frames, and highlights moving objects with a bounding box — displaying a real-time status on screen.

---

## 📸 Demo

> The system shows **"Normal"** when the scene is still and **"Moving Object Detected"** with a green bounding box when motion is found.

```
[Live Camera Feed]
  → Frame 1 captured as background reference
  → Each new frame compared to background
  → Motion area highlighted with green rectangle
  → Status label updated in real-time
```

---

## ⚙️ How It Works

1. **Background Reference** — Captures the first frame as a static background
2. **Grayscale + Blur** — Converts each frame to grayscale and applies Gaussian Blur to reduce noise
3. **Frame Differencing** — Finds the absolute difference between the background and current frame
4. **Thresholding** — Applies a binary threshold to isolate motion regions
5. **Contour Detection** — Detects contours of moving regions and draws bounding boxes

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| OpenCV | Real-time image & video processing |
| imutils | Frame resizing and contour utilities |

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/arunkumararavindhakshan05-sudo/Moving_object_detection_using_opencv.git
cd Moving_object_detection_using_opencv

# Install dependencies
pip install opencv-python imutils
```

---

## ▶️ Usage

```bash
python cameraTest.py
```

**Controls:**
- Press **`Q`** — Quit the camera feed

---

## 📁 Project Structure

```
Moving_object_detection_using_opencv/
│
├── cameraTest.py       # Main script
├── .gitignore
└── README.md
```

---

## 🔮 Future Improvements

- [ ] Add sensitivity/threshold configuration via command-line arguments
- [ ] Save video recording when motion is detected
- [ ] Send email/SMS alert on detection
- [ ] Multi-camera support

---

## 👤 Author

**Arunkumar Aravindhakshan**
🔗 [LinkedIn](https://linkedin.com/in/arunkumar-aravindhakshan) | [GitHub](https://github.com/arunkumararavindhakshan05-sudo)
