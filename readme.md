🧠 AI-Powered Study Monitoring System

An intelligent AI-powered study monitoring system built with Python, OpenCV, MediaPipe, and YOLOv8 to help students maintain focus and monitor their study sessions using computer vision.

The system analyzes the user's face, eyes, hands, and surroundings in real time and can provide audio alerts when signs of distraction or inactivity are detected.

✨ Features
👁️ Eye & Face Monitoring

Detects and tracks the user's face.

Monitors eye-related activity using facial landmarks.

Helps identify when the user is not properly focused on the screen.

✋ Hand Detection

Tracks hand movements using MediaPipe hand landmarks.

Can be used to identify distracting hand activity.

🎯 Object Detection

Uses YOLOv8 for real-time object detection.

Helps identify objects in the user's environment.

🔊 Audio Alerts

Plays warning sounds when specific conditions are detected.

Supports multiple audio files for different alerts.

📊 Real-Time Monitoring

Processes camera input continuously.

Provides an interactive study-monitoring experience.

🧠 Deep Learning & Computer Vision

Combines multiple AI and computer-vision techniques into one application.

Uses pre-trained deep learning models for real-time analysis.

🛠️ Technologies Used
Technology	Purpose
🐍 Python	Core programming language
👁️ OpenCV	Camera processing and computer vision
🤖 YOLOv8	Real-time object detection
🧍 MediaPipe	Face and hand landmark detection
🔊 Audio Processing	Study and distraction alerts
🧠 Deep Learning	Intelligent monitoring and analysis
📁 Project Structure
study_moniter/
│
├── app.py
├── requirements.txt
│
├── yolov8n.pt
├── face_landmarker.task
├── hand_landmarker.task
│
├── alarm.mp3
├── faudio.mp3
├── paudio.mp3
│
└── README.md

File Description
File	Description
app.py	Main application
requirements.txt	Python dependencies
yolov8n.pt	YOLOv8 Nano model
face_landmarker.task	MediaPipe face landmark model
hand_landmarker.task	MediaPipe hand landmark model
alarm.mp3	Alert sound
faudio.mp3	Face/distraction audio
paudio.mp3	Additional alert audio
🚀 Getting Started
1. Clone the Repository
git clone https://github.com/akashsingh41882-byte/study_moniter.git


Navigate to the project directory:

cd study_moniter

2. Create a Virtual Environment

It is recommended to use a virtual environment.

Windows
python -m venv venv


Activate the virtual environment:

venv\Scripts\activate

macOS / Linux
python3 -m venv venv


Activate the virtual environment:

source venv/bin/activate

3. Install Dependencies

Install all required Python packages:

pip install -r requirements.txt

4. Run the Application

Start the study monitoring system:

python app.py


Make sure your computer has a working webcam/camera available.

🎥 How It Works

The system follows a computer-vision-based monitoring pipeline:

                    ┌─────────────────┐
                    │  Webcam Input   │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Image Processing│
                    │     OpenCV      │
                    └────────┬────────┘
                             │
             ┌───────────────┼───────────────┐
             │               │               │
             ▼               ▼               ▼
       ┌───────────┐   ┌───────────┐   ┌───────────┐
       │Face / Eyes│   │   Hands   │   │  Objects  │
       │ Detection │   │ Detection │   │  YOLOv8   │
       └─────┬─────┘   └─────┬─────┘   └─────┬─────┘
             │               │               │
             └───────────────┼───────────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │  Focus Analysis │
                    └────────┬────────┘
                             │
                    ┌────────┴────────┐
                    │                 │
                    ▼                 ▼
               ┌─────────┐      ┌────────────┐
               │ Focused │      │ Distracted │
               └─────────┘      └──────┬─────┘
                                       │
                                       ▼
                                🔊 Audio Alert

🎯 Project Goal

The goal of this project is to create an AI-assisted study environment that helps students:

🎯 Maintain concentration while studying.

🚫 Reduce distractions.

📊 Monitor study behavior.

🔊 Receive real-time alerts.

🧠 Explore practical applications of computer vision and deep learning.

This project demonstrates how Artificial Intelligence and Computer Vision can be applied to education and productivity.

🔮 Future Improvements

The project can be extended with several additional features:

📈 Study-session analytics and reports

⏱️ Pomodoro timer integration

📊 Daily and weekly productivity dashboard

🗃️ Study-session history

🎯 Focus score calculation

📱 Web/mobile dashboard

🧠 Improved distraction detection

🔔 Customizable alert settings

☁️ Cloud-based study statistics

👤 Multi-user support

⚠️ Requirements

Before running the application, make sure you have:

🐍 Python 3.9 or higher

📷 A working webcam

💻 Windows, Linux, or macOS

🧠 Sufficient system resources for real-time computer vision

🌐 Internet connection for installing dependencies

🔐 Privacy

This project is designed for local computer-vision-based monitoring.

Camera input should be handled according to the implementation in app.py. Users should review how video and image data are processed before using the application in environments involving other people.

🤝 Contributing

Contributions are welcome! 🎉

If you would like to improve this project:

1. Fork the repository

Create your own fork of this repository on GitHub.

2. Create a new branch
git checkout -b feature/improvement

3. Make your changes

Implement your improvements or fixes.

4. Commit your changes
git add .
git commit -m "Add new improvement"

5. Push your branch
git push origin feature/improvement

6. Open a Pull Request

Create a Pull Request on GitHub describing your changes.

⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐ Star on GitHub.

Every star helps support the project! 🚀

👨‍💻 Author
Akash Singh

GitHub: @akashsingh41882-byte

📜 License

This project is currently intended for educational and personal use.

A formal open-source license can be added in the future.

<div align="center">
🧠 Built with Python, OpenCV, MediaPipe & YOLOv8

Made with ❤️ for smarter and more focused studying.

</div>
