# 🏋️‍♂️ Posture Pal

Welcome to **Posture Pal**! This is a real-time posture tracking web application designed to help you maintain good posture using your webcam. 

Our application uses an advanced machine learning model to analyze your body posture in real-time, providing immediate visual feedback directly through your browser.

## ✨ Features
- **Real-Time Feedback**: Get instant visual feedback on your posture using your webcam.
- **AI-Powered**: Uses a YOLOv5 machine learning model running on a lightning-fast FastAPI backend.
- **Interactive UI**: A beautiful, modern, and responsive frontend built with React and Vite.

## 👨‍💻 Developer
**Dhruv Ghugal**
- **Repository**: [Mega-Project-PosturePal-](https://github.com/DhruvGhugal/Mega-Project-PosturePal-)

---

## 🏗️ Project Structure

The project is divided into two main parts—the frontend interface and the backend AI server.

### 🎨 Frontend (`client/`)
Built using **React** and **Vite**, the frontend provides a sleek, responsive user interface.
- **`src/pages/`**: The main screens of the application (e.g., Dashboard, Login, Landing Page).
- **`src/components/`**: Reusable UI elements.
- **`src/features/camera/`**: Where the live webcam view and drawing logic happens.
- **`src/services/`**: Handles communication with the backend.

### 🧠 Backend (`server/`)
Built using **Python** and **FastAPI**, the backend acts as the brain of the application.
- Uses a **YOLOv5** machine learning model (`yolov5s.pt` / `yolov5n.pt`) to detect and analyze human poses.
- Receives video frames from the frontend, analyzes the posture, and sends back the results in real-time.

---

## 🚀 How to Run the Project

We have made running the project as incredibly easy as possible! You do not need to manually install any dependencies. 

1. Simply double-click the **`run_posture_pal.bat`** file in the root directory.
2. If this is your first time running it, the script will automatically create a virtual environment and download everything it needs (like React packages and PyTorch). 
3. It will launch two separate windows: one for the backend server and one for the frontend server.
4. Your browser will automatically open to `http://localhost:5173` where you can use Posture Pal!

---

## 💡 Notes
* The heavy dependency folders (`node_modules` and `venv`) are intentionally ignored by Git so that this repository stays incredibly fast and lightweight.
* Do not delete the `.pt` files in the server folder, as those are the core AI models used for posture detection.
