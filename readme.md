# ✋ Air Canvas using Hand Tracking (Python)

Air Canvas is a computer-vision–based application that allows users to **draw, erase, and change colors in mid-air using hand gestures**. It uses a webcam for real-time input and tracks hand landmarks using **MediaPipe**, enabling a natural, touch-free drawing experience.

---

## 🎯 Features

- ✏️ Draw in the air using your **index finger**
- 🎨 Select colors using **index + middle finger**
- 🧽 Erase drawings using **four fingers**
- 🖐️ Real-time hand landmark detection
- 🎥 Live webcam feed using OpenCV
- 🧼 Clear canvas with a keyboard shortcut
- 🚪 Exit the application safely

---

## 🛠 Tech Stack

- **Python**
- **OpenCV**
- **MediaPipe**
- **NumPy**

---

## 📦 Requirements

- Python **3.8 – 3.11**
- pip (Python package manager)
- Webcam (built-in or external)

---

## 🚀 Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/air-canvas.git
cd air-canvas
```

---

### 2️⃣ Create and Activate a Virtual Environment (Recommended)

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

You should see `(venv)` in your terminal after activation.

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️⃣ Run the Application

```bash
python air_canvas.py
```

> Replace `air_canvas.py` with your actual Python file name if it differs.

---

## 🖐️ Gesture Controls

| Gesture                  | Action           |
| ------------------------ | ---------------- |
| ☝️ Index finger          | Draw             |
| ✌️ Index + Middle finger | Select color     |
| 🖐️ Four fingers         | Erase            |
| **C key**                | Clear canvas     |
| **Q key**                | Quit application |

---

## 🎨 Color Palette

The color palette appears at the **top of the screen**.

Available colors:

- Purple
- Blue
- Green
- Yellow
- Eraser (Black)

To select a color:

- Raise **index + middle finger**
- Move your hand over the desired color block

---

## 📁 Project Structure

```
├── air_canvas.py
├── requirements.txt
└── README.md
```

---

## ❗ Common Issues & Fixes

### MediaPipe Installation Fails

Make sure your Python version is compatible:

```bash
python --version
```

Use Python **≤ 3.11**.

---

### Webcam Not Opening

Try changing the camera index in the code:

```python
cv2.VideoCapture(1)
```

---

### Poor Hand Detection

- Ensure good lighting
- Keep your hand fully visible to the camera
- Avoid cluttered backgrounds

---

## 🧹 Deactivate Virtual Environment

```bash
deactivate
```

---

## 📌 Best Practices

- ❌ Do NOT upload the `venv/` folder to GitHub
- ✅ Always include `requirements.txt`
- ✅ Use `.gitignore` for clean repositories

Example `.gitignore`:

```gitignore
venv/
__pycache__/
.env
```

---

## 🚀 Future Improvements

- Save drawings as image files
- Add gesture-based undo/redo
- Support multiple hands
- Improve UI and color selection
- Optimize performance for low-end systems

---

## 📄 License

This project is open-source and intended for learning, experimentation, and personal use.

