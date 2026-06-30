# SkillCraft_Task04_HandGesture
Developed a Hand Gesture Recognition system using Python, OpenCV, and MediaPipe to detect and classify hand gestures in real time. Created a custom landmark-based dataset for training machine learning models, enabling accurate gesture recognition for human-computer interaction applications.
# ✋ Hand Gesture Recognition using MediaPipe and OpenCV

## 📌 Project Overview

The **Hand Gesture Recognition System** is a computer vision and machine learning project developed using **Python**, **OpenCV**, and **Google MediaPipe**. The project detects and tracks a user's hand in real time through a webcam, extracts 21 hand landmarks, and recognizes different hand gestures based on the positions of these landmarks.

In addition to real-time recognition, the project also includes a **dataset collection module** that allows users to generate a custom dataset of hand landmarks. This dataset can later be used to train machine learning models such as Support Vector Machine (SVM), Random Forest, Decision Tree, or Neural Networks for more advanced gesture recognition tasks.

The project demonstrates the practical application of computer vision, machine learning, and human-computer interaction by enabling intuitive communication between users and computers through hand gestures.

---

# 🎯 Objectives

* Develop a real-time hand gesture recognition system.
* Detect and track hands using MediaPipe.
* Extract hand landmark coordinates for gesture analysis.
* Generate a custom dataset for machine learning.
* Recognize common hand gestures accurately.
* Provide a foundation for future AI-based gesture recognition projects.

---

# 🚀 Features

* Real-time hand detection using a webcam.
* Detection of 21 hand landmarks.
* Landmark visualization with connections.
* Gesture classification using landmark positions.
* Custom dataset generation in CSV format.
* Supports multiple gesture categories.
* Easy-to-understand and modular code structure.
* Lightweight and fast execution.
* Suitable for beginners and academic projects.

---

# 🛠️ Technologies Used

* **Programming Language:** Python
* **Computer Vision:** OpenCV
* **Hand Tracking:** Google MediaPipe
* **Dataset Format:** CSV
* **Machine Learning Ready:** Landmark-based dataset
* **Development Environment:** Visual Studio Code

---

# 📂 Project Structure

```
HandGestureRecognition/
│
├── collect_dataset.py          # Dataset collection script
├── hand_gesture.py             # Real-time gesture recognition
├── hand_landmarker.task        # MediaPipe model
├── hand_gesture_dataset.csv    # Generated dataset
├── requirements.txt            # Required libraries
├── README.md                   # Project documentation
└── screenshots/                # Output screenshots (optional)
```

---

# 📋 Requirements

Install Python 3.10 or above.

Install the required libraries:

```bash
pip install opencv-python
pip install mediapipe
pip install numpy
```

Or install everything at once:

```bash
pip install -r requirements.txt
```

---

# ⚙️ How It Works

### Step 1: Webcam Initialization

The system accesses the default webcam using OpenCV.

### Step 2: Hand Detection

MediaPipe detects the user's hand from each video frame.

### Step 3: Landmark Extraction

MediaPipe extracts 21 hand landmarks.

Each landmark contains:

* X Coordinate
* Y Coordinate
* Z Coordinate

These coordinates describe the position of every finger joint.

### Step 4: Gesture Recognition

The program compares the positions of the landmarks to determine whether the hand is showing:

* Open Palm
* Fist
* Thumbs Up
* Other Gesture

### Step 5: Display Output

The detected gesture is displayed on the webcam screen along with the hand landmarks.

---

# 📊 Dataset Collection

The project also contains a separate dataset collection script.

Instead of saving images, it saves the numerical coordinates of the detected landmarks.

Each sample contains:

* Gesture Label
* 21 Hand Landmarks
* X, Y and Z Coordinates

Total Features:

* 21 Landmarks
* 3 Coordinates per Landmark

Total = **63 Features**

Example:

```
Label,x0,y0,z0,x1,y1,z1,...,x20,y20,z20
Open Palm,...
Fist,...
Thumbs Up,...
```

The dataset is stored as:

```
hand_gesture_dataset.csv
```

This dataset can later be used to train custom machine learning models.

---

# 🧠 Supported Gestures

Currently the project recognizes:

* ✋ Open Palm
* ✊ Fist
* 👍 Thumbs Up
* 🤚 Other Gesture

More gestures can easily be added by modifying the gesture classification logic.

---

# ▶️ Running the Project

### Clone the repository

```bash
git clone https://github.com/your-username/HandGestureRecognition.git
```

### Navigate to the project

```bash
cd HandGestureRecognition
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the gesture recognition

```bash
python hand_gesture.py
```

### Run dataset collection

```bash
python collect_dataset.py
```

---

# 📈 Applications

This project has many practical applications, including:

* Human Computer Interaction (HCI)
* Touchless Computer Control
* Smart Home Automation
* Virtual Mouse Systems
* Sign Language Recognition
* Interactive Games
* Educational Projects
* AI Research
* Robotics
* Healthcare Assistance
* Gesture-Based Presentation Control
* Contactless User Interfaces

---

# 📸 Output

The application displays:

* Live webcam feed
* Hand landmark visualization
* Hand skeleton connections
* Detected gesture label
* Real-time tracking

You can also add screenshots inside the **screenshots/** folder for better project presentation.

---

# 🔮 Future Enhancements

Some possible improvements include:

* Support for more hand gestures.
* Two-hand gesture recognition.
* Deep learning-based classification.
* Gesture-controlled media player.
* Gesture-based volume control.
* Virtual drawing application.
* Sign language sentence recognition.
* Mouse and keyboard control using gestures.
* Mobile application integration.
* Higher accuracy using custom-trained models.

---

# 📚 Learning Outcomes

Through this project, the following concepts can be understood:

* Computer Vision
* Image Processing
* Hand Landmark Detection
* MediaPipe Framework
* OpenCV Programming
* Dataset Creation
* Feature Extraction
* Machine Learning Preparation
* Real-Time Video Processing
* Human-Computer Interaction

---

# 🤝 Contribution

Contributions are welcome.

If you would like to improve this project:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push to your branch.
5. Submit a Pull Request.

Suggestions and improvements are always appreciated.

---

# 📄 License

This project is intended for educational, learning, and research purposes. Feel free to use, modify, and extend the project with appropriate attribution.

---

# 👨‍💻 Author

**Panthangi Surya Tej**

This project was developed as part of my learning journey in **Computer Vision**, **Machine Learning**, and **Artificial Intelligence**. It demonstrates real-time hand tracking, gesture recognition, and dataset generation using Python, OpenCV, and MediaPipe while serving as a foundation for future AI-powered gesture recognition applications.
