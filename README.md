# 🧍 Posture Detection App

A full-stack computer vision application for **real-time and video-based posture analysis** using **MediaPipe Pose Estimation, OpenCV, FastAPI, React, and WebSockets**.

The application uses **rule-based posture analysis** to identify incorrect sitting and squat postures and provides real-time visual feedback to the user.

## 🚀 Features

- 🎥 **Real-Time Posture Analysis** – Monitor posture continuously using a webcam.
- 📹 **Video Upload Analysis** – Upload recorded videos for posture analysis.
- 🧍 **Multiple Posture Types** – Supports sitting and squat posture analysis.
- 📐 **Rule-Based Detection** – Detect incorrect posture using customizable angle, alignment, and position thresholds.
- ⚠️ **Visual Feedback** – Displays posture status and alerts directly on the video/webcam feed.
- 📊 **Analysis Results** – View detailed posture analysis results after processing.
- 📄 **Export Results** – Export posture analysis data as JSON.
- 📱 **Responsive Interface** – Designed for desktop and mobile devices.

## 🛠️ Tech Stack

### Backend

- **Python**
- **FastAPI** – REST API development
- **MediaPipe** – Pose estimation
- **OpenCV** – Computer vision and video processing
- **WebSockets** – Real-time communication
- **Uvicorn** – ASGI server

### Frontend

- **React 18**
- **TypeScript**
- **React Webcam** – Webcam integration
- **Axios** – HTTP client
- **WebSocket** – Real-time communication
- **CSS Grid & Flexbox** – Responsive UI

## 🧠 Posture Analysis

The application uses human body landmarks detected through **MediaPipe Pose** and applies predefined rules to determine posture quality.

### 🪑 Sitting Posture

The system evaluates:

- **Neck Forward Position** – Flags excessive forward neck positioning when the neck angle exceeds **30°**.
- **Back Straightness** – Detects slouching using shoulder and hip alignment.
- **Shoulder Level** – Checks whether the shoulders are positioned at a balanced level.

### 🏋️ Squat Posture

The system evaluates:

- **Knee Over Toe** – Detects when the knee moves beyond the toe position.
- **Back Angle** – Flags incorrect back positioning when the shoulder-hip-knee angle is below **150°**.
- **Squat Depth** – Evaluates knee angle to determine whether sufficient squat depth is achieved.

📂 Project Structure

posture-detection-app/
│
├── backend/
│   ├── main.py
│   ├── posture_detector.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── App.tsx
│   │   ├── WebcamCapture.tsx
│   │   ├── VideoUpload.tsx
│   │   ├── AnalysisResults.tsx
│   │   ├── api.ts
│   │   ├── types.ts
│   │   └── App.css
│   │
│   ├── package.json
│   └── tsconfig.json
│
└── README.md

⚙️ Installation & Setup
Prerequisites

Make sure the following are installed:

Python 3.9+
Node.js 16+
npm or Yarn


