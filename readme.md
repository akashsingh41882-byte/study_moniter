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

Combines multiple AI/computer-vision techniques into one application.

🛠️ Technologies Used
Technology	Purpose
🐍 Python	Core programming language
👁️ OpenCV	Camera processing and computer vision
🤖 YOLOv8	Object detection
🧍 MediaPipe	Face and hand landmark detection
🔊 Audio Processing	Study/distraction alerts
🧠 Deep Learning	Intelligent monitoring
📁 Project Structure
study_moniter/
│
├── app.py                  # Main application
├── requirements.txt        # Python dependencies
│
├── yolov8n.pt              # YOLOv8 Nano model
├── face_landmarker.task    # MediaPipe face landmark model
├── hand_landmarker.task    # MediaPipe hand landmark model
│
├── alarm.mp3               # Alert sound
├── faudio.mp3              # Face/distraction audio
├── paudio.mp3              # Additional alert audio
│
└── README.md               # Project documentation

🚀 Getting Started
1. Clone the Repository
git clone https://github.com/akashsingh41882-byte/study_moniter.git


Navigate into the project directory:

cd study_moniter

2. Create a Virtual Environment

It is recommended to use a virtual environment.

Windows
python -m venv venv


Activate it:

venv\Scripts\activate

macOS / Linux
python3 -m venv venv

source venv/bin/activate

3. Install Dependencies

Install the required Python packages:

pip install -r requirements.txt

4. Run the Application

Start the monitoring system using:

python app.py


Make sure your computer has a working webcam/camera available.

🎥 How It Works

The system follows a computer-vision-based monitoring pipeline:

             ┌─────────────────┐
             │   Webcam Input  │
             └────────┬────────┘
                      │
                      ▼
             ┌─────────────────┐
             │ Image Processing│
             │    OpenCV       │
             └────────┬────────┘
                      │
          ┌───────────┼───────────┐
          ▼           ▼           ▼
     Face/Eyes      Hands      Objects
     Detection    Detection    YOLOv8
          │           │           │
          └───────────┼───────────┘
                      ▼
             ┌─────────────────┐
             │  Focus Analysis │
             └────────┬────────┘
                      │
              ┌───────┴───────┐
              ▼               ▼
          Focused         Distracted
                              │
                              ▼
                       🔊 Audio Alert

🎯 Project Goal

The goal of this project is to create an AI-assisted environment that helps students:

Maintain concentration while studying.

Reduce distractions.

Monitor study behavior.

Receive real-time alerts.

Experiment with practical applications of computer vision and deep learning.

This project is also intended as a practical demonstration of how AI and computer vision can be applied to education and productivity.

🔮 Future Improvements

Some possible improvements for future versions include:

📈 Study-session analytics and reports

⏱️ Pomodoro timer integration

📊 Daily/weekly productivity dashboard

🗃️ Study-session history

🎯 Focus score calculation

📱 Web/mobile dashboard

🧠 Improved distraction detection

🔔 Customizable alert settings

☁️ Cloud-based study statistics

👤 Multi-user support

⚠️ Requirements

Before running the application, make sure you have:

Python 3.9+

A working webcam

Windows / Linux / macOS

Sufficient system resources for real-time computer vision

Internet connection for initial dependency installation

🔐 Privacy

This project is designed for local computer-vision-based monitoring.

Camera input should be processed according to the implementation in app.py. Users should review and understand how video/images are handled before using the application in environments involving other people.

🤝 Contributing

Contributions are welcome!

If you would like to improve this project:

Fork the repository.

Create a new branch.

git checkout -b feature/improvement


Make your changes.

Commit your changes.

git add .
git commit -m "Add new improvement"


Push your branch.

git push origin feature/improvement


Open a Pull Request.

⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub.

👨‍💻 Author

Akash Singh

GitHub: @akashsingh41882-byte

📜 License

This project is currently available for educational and personal use.

A formal open-source license can be added in the future.