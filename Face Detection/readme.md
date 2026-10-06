# 👁️ Real-Time Face Detection with OpenCV

A simple **real-time face detection system** built with **Python and OpenCV** that uses a webcam to detect human faces and highlights them with bounding boxes.

---

## ✨ Features

* 🎥 Real-time webcam video
* 👤 Detects multiple faces
* 🧠 Haar Cascade face detection
* 📦 Built with OpenCV
* ⚡ Lightweight and fast
* 🖼️ Draws bounding boxes around detected faces

---

## 🛠️ Technologies

| Technology      | Purpose              |
| --------------- | -------------------- |
| 🐍 Python       | Programming language |
| 👁️ OpenCV      | Computer vision      |
| 🧠 Haar Cascade | Face detection       |
| 📷 Webcam       | Real-time input      |

---

## 📂 Project Structure

```text
Face Detection/
│
└── face_detection.ipynb
```

---

## 🚀 How It Works

The program follows a simple pipeline:

```text
Webcam
   ↓
Capture Frame
   ↓
Convert to Grayscale
   ↓
Haar Cascade Detector
   ↓
Detect Faces
   ↓
Draw Bounding Boxes
   ↓
Display Result
```

---

## ⚙️ Installation

Install OpenCV:

```bash
pip install opencv-python
```

---

## ▶️ Run the Project

Open the notebook:

```text
face_detection.ipynb
```

Run the cells and allow the application to access your webcam.

Press **`A`** to stop the face detection window.

---

## 🔍 Detection Parameters

The detector uses:

```python
faces = face_cascade.detectMultiScale(
    gray,
    scaleFactor=1.1,
    minNeighbors=5,
    minSize=(30, 30)
)
```

* **`scaleFactor=1.1`** → Detects faces at different sizes.
* **`minNeighbors=5`** → Controls detection confidence.
* **`minSize=(30, 30)`** → Ignores faces smaller than 30×30 pixels.

---

## 🖼️ Output

Detected faces are highlighted using a **blue bounding box**:

```text
        ┌──────────────┐
        │              │
        │     FACE     │
        │              │
        └──────────────┘
```

---

## 📌 Note

This project uses the **Haar Cascade Classifier**, which is a traditional computer-vision approach to object detection. It is lightweight and suitable for real-time applications, although modern deep-learning detectors can provide better accuracy in challenging conditions.

---

## 👩‍💻 Author

**Alina**

Built as part of my **Python & Computer Vision projects**.

---

⭐ If you found this project useful, consider giving the repository a star!
