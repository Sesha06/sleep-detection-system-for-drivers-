# sleep-detection-system-for-drivers-
A real-time driver drowsiness detection system using OpenCV and MediaPipe FaceMesh to monitor eye openness and alert when eyes are closed. Detects eye status using facial landmarks and visualizes results live from the webcam feed.
Perfect — your file `hryhtrh.py` is a **Driver Eye Monitoring System** that uses OpenCV and MediaPipe to detect whether a person’s eyes are open or closed in real time from a webcam feed.


### 📝 **GitHub Repository Description**

> A real-time driver drowsiness detection system using OpenCV and MediaPipe FaceMesh to monitor eye openness and alert when eyes are closed. Detects eye status using facial landmarks and visualizes results live from the webcam feed.

---

### 📘 **README.md**

````markdown
# Driver Eye Monitoring System 🚗👁️

A Python-based real-time **Driver Drowsiness Detection System** using **OpenCV** and **MediaPipe FaceMesh**.  
It monitors the user’s eye openness from a webcam feed and determines whether the driver’s eyes are **open** or **closed**, which can be used to alert in case of drowsiness.

---

## 🧠 Features

- Real-time face and eye detection using MediaPipe
- Calculates eye openness (EAR-like method)
- Displays live webcam feed with eye landmarks
- Highlights eyes in **green** (open) or **red** (closed)
- Works efficiently on most standard webcams

---

## 🛠️ Requirements

Install the required libraries before running:

```bash
pip install opencv-python mediapipe numpy
````

---

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/driver-eye-monitoring.git
   cd driver-eye-monitoring
   ```

2. Run the Python script:

   ```bash
   python hryhtrh.py
   ```

3. A window will open showing your webcam feed:

   * **Green text / circles** → Eyes are open
   * **Red text / circles** → Eyes are closed

4. Press **ESC** to quit the program.

---

## ⚙️ How It Works

1. The program uses **MediaPipe’s FaceMesh** model to detect 468 facial landmarks.
2. Eye landmarks (specific index points) are extracted for both eyes.
3. The vertical and horizontal distances between key eye landmarks are used to estimate the **Eye Aspect Ratio (EAR)**.
4. If the average eye openness falls below a threshold (0.2 by default), it is considered **closed**.

---

## 📸 Example Output

| Status      | Visualization                         |
| ----------- | ------------------------------------- |
| Eyes Open   | 🟢 Green outline and “EYES OPEN” text |
| Eyes Closed | 🔴 Red outline and “EYES CLOSED” text |

---

## 🚀 Future Improvements

* Add an **audio alert** for prolonged eye closure
* Integrate with **Raspberry Pi** or **IoT** systems
* Use **Blink frequency** or **PERCLOS** (Percentage of Eye Closure) for advanced fatigue detection
* Log drowsiness data for analytics

---

## 🧩 Tech Stack

* **Language:** Python
* **Libraries:** OpenCV, MediaPipe, NumPy
* **Model:** FaceMesh from Google MediaPipe

---

## 👨‍💻 Author

**Sesha**
B.Tech CSE, SRM University – Kattankulathur
Passionate about AI, Computer Vision, and Automation.

---

Would you like me to add a **sound alert feature** (a beep when eyes remain closed for a few seconds)? It would make this project look even more polished and practical for a GitHub demo.
```
