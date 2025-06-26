# 🦾 ChalChitra: Agentic Vision Assistant for the Visually Impaired

> “Empowering vision without sight – through voice, gesture, and AI.”

LucidNav is a **multimodal, agentic AI-powered navigation and scene interpretation assistant** tailored for the visually impaired. With an intuitive blend of **real-time computer vision, gesture recognition, voice narration**, and **emergency response**, this project transforms ordinary webcams into smart assistant eyes – powered by open-source intelligence.

---

## 🧠 What Makes ChalChitra Unique?

- 🎯 **Scene Interpreter**: Detects multiple objects with directional and distance-based awareness. Example: “A person to your left at 2.3 meters.”
- ✋ **Gesture-Based Commands**: Detects peace signs, thumbs up, fists, and more using MediaPipe for hands-free interaction.
- 🧠 **Emotion-Aware Agent**: Recognizes human facial emotions using `DeepFace` and includes them in environment narration.
- 📖 **Live OCR for Navigation**: Reads out signboards, posters, or door labels in real-time using EasyOCR.
- 📡 **Emergency SOS Trigger (Double Tap)**: Sends the user's live location via Twilio to family/friends with a simple screen double-tap.
- 🧭 **Distance + Directional Feedback**: Calculates estimated distance to known objects and gives left/center/right orientation feedback.
- 📢 **Text-to-Speech Scene Narration**: Converts all detections and environmental summaries into natural voice feedback using `pyttsx3`.
- 💬 **Agentic Intelligence Layer**: Agent-like logic flow determines what to narrate, when to narrate, and avoids repetitive or cluttered feedback.

---

## 🚀 Tech Stack

| Module             | Description                                                       |
|--------------------|-------------------------------------------------------------------|
| `YOLOv8`           | Real-time object detection and labeling.                         |
| `MediaPipe`        | Gesture detection through hand landmark tracking.                |
| `DeepFace`         | Facial expression analysis.                                       |
| `EasyOCR`          | Lightweight OCR module to extract readable text.                 |
| `OpenCV`           | Frame processing and rendering annotations.                      |
| `Tkinter`          | GUI to simulate vision stream and emergency triggers.            |
| `pyttsx3`          | Offline text-to-speech engine for audio feedback.                |
| `Geocoder`         | Fetches live geolocation using IP.                               |
| `Twilio`           | Sends SMS-based alerts to family contacts with location links.   |

---

## 📌 Features At a Glance

- Real-time object + gesture detection.
- Voice-based environment narration.
- SOS detection with geolocation.
- OCR of visible texts and boards.
- Emotion and facial mood reading.
- Indoor-aware navigation logic support (extensible to "Take me to kitchen" etc.).

---

## 📦 Installation

```bash
git clone https://github.com/your-username/lucidnav.git
cd lucidnav
pip install -r requirements.txt
python main.py
