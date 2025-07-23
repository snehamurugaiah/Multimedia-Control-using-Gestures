# 🖐️ Hand Gesture Based System Control using MediaPipe, OpenCV and Python

This project enables **touchless control of system functions** using real-time **hand gesture recognition** powered by **MediaPipe**, **OpenCV**, and **Python**. It detects specific gestures via webcam and maps them to useful system actions like adjusting **volume**, **brightness**, **browser navigation**, and even **muting/unmuting** the device — making interactions more natural, fun, and accessible.


## 🚀 Key Features

| Feature | Description |
|--------|-------------|
| 🔊 Volume Control | Adjust system volume by changing the distance between thumb and index finger on the **right hand**. |
| 🔅 Brightness Control | Adjust screen brightness using **left-hand** gestures. |
| 🌐 Launch Web Browser | Raise all fingers on the **right hand** to open Google in the default browser. |
| 🔇 Mute/Unmute | Raise the middle finger on your **right hand** to toggle mute state. |
| 🔁 Switch Browser Tabs | Swipe index finger left/right to switch between tabs. |
| 👀 Visual Feedback | Visual overlays show gesture detections (circles, lines, and text). |

## 🧠 How It Works

The system uses **MediaPipe**'s hand tracking model to detect 21 hand landmarks in real-time. Based on their relative positions and distances, specific gestures are recognized:

- **Finger tip landmarks** like `id 4` (thumb) and `id 8` (index) are used for measuring distances.
- **Swipe gestures** are detected using horizontal movement (`delta_x`) of index finger.
- **Gesture recognition** triggers actions using `pyautogui`, `screen_brightness_control`, and OS-level commands.



## 📷 Demo Preview

> 📌 You can add screenshots or a GIF here demonstrating:
> - Swiping to switch browser tabs
> - Pinching to change brightness
> - Raising fingers to mute or open browser


## 🛠️ Tech Stack

- **Python 3.7+**
- **MediaPipe** – Hand landmark detection
- **OpenCV** – Video capture and overlay
- **PyAutoGUI** – Volume & tab control
- **screen_brightness_control** – Adjust brightness
- **nircmd** (Windows only) – Mute/Unmute system volume
- **Webbrowser Module** – Opens browser using gestures



