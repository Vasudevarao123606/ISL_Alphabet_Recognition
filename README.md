# 🇮🇳 Indian Sign Language (ISL) Alphabet Recognition

A Python-based computer vision and machine learning project that recognizes **Indian Sign Language (ISL) alphabet hand gestures** from image/video input. The project uses hand-landmark features and a trained machine-learning model to predict the corresponding ISL alphabet.

> **Note:** The large `isl_dataset/` image dataset is intentionally excluded from this repository through `.gitignore` to keep the GitHub repository lightweight.

---

## 📌 Project Description

Communication can be difficult for people who do not understand sign language. This project aims to provide a simple foundation for recognizing **Indian Sign Language alphabet gestures** using computer vision and machine learning.

The system processes a hand image/video frame, extracts meaningful hand-landmark information, converts those landmarks into features, and passes the features to a trained classification model. The predicted alphabet is then displayed by the application.

---

## ✨ Features

- 🤟 Recognition of ISL alphabet hand gestures
- 📷 Image/video-based hand gesture processing
- 🖐️ Hand-landmark feature extraction
- 🧹 Feature preprocessing
- 🤖 Trained machine-learning classification model
- 📊 CSV-based landmark datasets
- 🐍 Python implementation
- 🚀 Simple application entry point through `app.py`
- 📦 Dependency management using `requirements.txt`

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Main programming language |
| **Computer Vision** | Processing hand/gesture input |
| **Hand Landmark Detection** | Extracting hand key-point information |
| **Machine Learning** | Classifying ISL alphabet gestures |
| **NumPy / Pandas** | Data and feature processing |
| **Pickle** | Loading the trained model |
| **CSV** | Storing landmark features |
| **Git & GitHub** | Version control and project hosting |

> The exact Python packages used by the project are listed in `requirements.txt`.

---

## 📁 Project Structure

```text
ISL_Alphabet_Recognition/
│
├── app.py
├── preprocess.py
├── extract_features.py
├── train_models.py
│
├── requirements.txt
├── isl_landmarks.csv
├── isl_landmarks_processed.csv
├── isl_model.pkl
│
├── isl_dataset/                 # Local dataset (not uploaded to GitHub)
│
└── .gitignore
```

### Main Files

- **`app.py`** — Main application used for ISL alphabet recognition.
- **`preprocess.py`** — Performs preprocessing required before model training/prediction.
- **`extract_features.py`** — Extracts hand-landmark features from the input data.
- **`train_models.py`** — Trains the machine-learning model.
- **`isl_landmarks.csv`** — Landmark feature data.
- **`isl_landmarks_processed.csv`** — Processed landmark data.
- **`isl_model.pkl`** — Saved trained classification model.
- **`requirements.txt`** — Python dependencies required to run the project.

---

## ⚙️ How ISL Recognition Works

The overall workflow can be represented as:

```text
Input Image / Video
        │
        ▼
Hand Detection
        │
        ▼
Hand Landmark Extraction
        │
        ▼
Feature Preprocessing
        │
        ▼
Trained ML Model
        │
        ▼
Predicted ISL Alphabet
```

### Step-by-step

1. **Input**
   - The application receives an image/video frame containing an ISL hand gesture.

2. **Hand Detection**
   - The hand is detected from the input.

3. **Landmark Extraction**
   - Important points/landmarks from the hand are extracted.
   - These landmarks provide a numerical representation of the gesture.

4. **Preprocessing**
   - The extracted features are processed into the format expected by the trained model.

5. **Classification**
   - `isl_model.pkl` is loaded and used to classify the processed hand features.

6. **Prediction**
   - The model predicts the corresponding ISL alphabet.

---

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/Vasudevarao123606/ISL_Alphabet_Recognition.git
```

### 2. Open the project directory

```bash
cd ISL_Alphabet_Recognition
```

### 3. Create a virtual environment

Windows:

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

Linux/macOS:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

From the project directory, run:

```bash
python app.py
```

Follow the instructions provided by the application.

> If your application requires a camera, make sure your webcam is connected and that Python has permission to access it.

---

## 📸 Screenshots

Add screenshots of your application here.

Recommended screenshots:

### Application Interface

Place an image such as:

```text
screenshots/app-interface.png
```

Then add:

```markdown
![Application Interface](screenshots/app-interface.png)
```

### ISL Alphabet Prediction

Place an image such as:

```text
screenshots/prediction.png
```

Then add:

```markdown
![ISL Alphabet Prediction](screenshots/prediction.png)
```

> **Tip:** Create a `screenshots` folder in the repository and add 2–3 clear screenshots of the working application.

---

## 🧠 Model

The trained model is stored as:

```text
isl_model.pkl
```

The model receives processed hand-landmark features and predicts the corresponding ISL alphabet class.

The training-related code is available in:

```text
train_models.py
```

---

## 📊 Dataset

The project was developed using an ISL alphabet image dataset.

The complete image dataset is **not included in this GitHub repository** because it contains approximately **26,000 images (~845 MB)**.

Instead, the repository contains the generated landmark/feature CSV files required by the project.

If the dataset is required to retrain the model, place the dataset locally in:

```text
isl_dataset/
```

before running the training pipeline.

---

## 🔄 Training Workflow

If you have the dataset available locally, the general workflow is:

```text
ISL Image Dataset
       │
       ▼
Preprocessing
       │
       ▼
Landmark / Feature Extraction
       │
       ▼
Processed Feature Dataset
       │
       ▼
Model Training
       │
       ▼
isl_model.pkl
```

Relevant scripts:

```bash
python preprocess.py
python extract_features.py
python train_models.py
```

Run these according to the workflow implemented in the project.

---

## 🔮 Future Improvements

- Improve recognition accuracy
- Support more real-time gestures
- Add sentence/word-level sign recognition
- Add confidence scores for predictions
- Improve handling of different lighting and backgrounds
- Deploy as a web or mobile application
- Add a larger and more diverse dataset
- Support continuous real-time sign recognition

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Push the branch.
6. Open a Pull Request.

---

## 📜 License

No license has been added to this repository yet.

If you plan to make the project open source, consider adding an appropriate license such as MIT after confirming that it fits your project's requirements and dataset/model usage.

---

## 👨‍💻 Author

**Vasudevarao123606**

GitHub:  
https://github.com/Vasudevarao123606

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.
[README.md](https://github.com/user-attachments/files/33746681/README.md)
