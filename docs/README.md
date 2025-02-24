# AI-Based Stroke Rehabilitation

## Project Overview

AI-Based Stroke Rehabilitation is a Python application designed to assist stroke survivors in regaining motor function through **AI-driven motion tracking**. The system employs **MediaPipe and OpenCV** to facilitate real-time hand tracking and gesture recognition, enabling patients to perform rehabilitation exercises remotely while receiving **instant feedback** to enhance their recovery process.

## Problem Statement

Stroke survivors often encounter several challenges in rehabilitation, including:

- **Limited access** to physical therapy centers due to mobility constraints or financial burdens.
- **Lack of real-time feedback** when performing home-based exercises, reducing effectiveness.
- **High costs** associated with specialized VR-based rehabilitation tools.
- **Slow recovery** due to irregular therapy sessions and lack of engagement.

This project addresses these challenges by providing a **cost-effective, AI-based rehabilitation system** that enhances accessibility and engagement.

## Key Features

- **Hand Tracking & Motion Analysis** using MediaPipe and OpenCV for precise movement detection.
- **AI-Powered Real-Time Feedback** to provide corrective guidance on hand movements.
- **Gamification Elements** to promote engagement and adherence to rehabilitation exercises.
- **Remote Monitoring** via a Flask-based web API to allow healthcare providers to track patient progress.
- **Data Visualization** to analyze and illustrate patient improvement over time.

## Technology Stack

- **Python** – Core programming language for implementation.
- **MediaPipe & OpenCV** – Hand tracking and gesture recognition.
- **Flask** – Web framework for remote monitoring and data storage.
- **NumPy & Pandas** – Data processing and analytics.
- **Matplotlib** – Visualization of patient progress.
- **Pygame** – Interactive exercises for gamification.

## Project Structure

```
ai-stroke-rehab/
│── src/                     # Source code
│   ├── hand_tracking.py        # MediaPipe-based hand tracking module
│   ├── gesture_recognition.py  # Gesture detection and classification
│   ├── ai_feedback.py          # AI-driven feedback for movement correction
│   ├── game_exercises.py       # Gamified rehabilitation exercises
│   ├── remote_monitoring.py    # Data storage and visualization module
│   ├── app.py                  # Main entry point of the application
│
│── models/                   # Machine Learning models (if required)
│   ├── gesture_model.pkl       # Pretrained gesture recognition model
│
│── data/                     # Stores user session data
│   ├── movements.csv           # Raw movement data collected from users
│   ├── progress_reports/       # Processed patient analytics
│
│── assets/                   # UI & Audio assets
│   ├── sounds/                 # Audio feedback (e.g., "Raise your hand higher")
│   ├── icons/                  # UI elements and buttons
│
│── docs/                     # Documentation and reports
│   ├── README.md               # Project overview
│   ├── setup_guide.md          # Installation and setup instructions
│   ├── api_docs.md             # API documentation (if applicable)
│
│── requirements.txt             # List of dependencies (OpenCV, MediaPipe, Flask, etc.)
│── .gitignore                   # Ignore unnecessary files
│── LICENSE                      # Open-source license information
│── README.md                    # General project documentation
```

## Installation & Setup

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/ai-stroke-rehab.git
cd ai-stroke-rehab
```

2. **Create a virtual environment (recommended):**

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. **Install dependencies:**

```bash
pip install -r requirements.txt
```

4. **Run the application:**

```bash
python src/app.py
```

## API Usage (Flask for Remote Monitoring)

The project includes a **Flask API** for remote tracking of patient progress. To start the API:

```bash
python src/remote_monitoring.py
```

The API will be accessible at `http://localhost:5000/`.

## Future Enhancements

- **Improve motion tracking accuracy** using Kalman Filters to reduce noise.
- **Develop AI-based gesture classification** for a wider range of rehabilitation exercises.
- **Integrate cloud storage** to allow healthcare professionals to monitor patient progress remotely.

## License

This project is licensed under the MIT License.

---

### Need Assistance?

For inquiries or contributions, please open an issue or reach out to the development team.

