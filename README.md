# 🧠 EEG Emotion Recognition Using Machine Learning

## 📘 Overview
This project predicts human emotions from EEG (Electroencephalogram) brainwave signals using Deep Learning.  
It features a **Flask-based web app** that allows users to input EEG signal values — *Attention*, *Meditation*, *Eye Blink*, and *Average* — and outputs the predicted **emotion** and its **intensity**.

---

## 🚀 Features
- Preprocessing of EEG dataset  
- Deep Learning model for emotion classification  
- Intensity prediction using regression  
- Flask web app interface for real-time predictions  
- Responsive front-end design with background visuals  
- 7 Emotion categories:
  - **Concentrated**
  - **Drunker**
  - **Excited**
  - **Fear**
  - **Happy**
  - **Relaxed**
  - **Sad**

---

## 🧩 Project Structure
EEG_Emotion_Recognition/
│
├── preprocess.py # Loads and preprocesses EEG data
├── train_model.py # Trains the models
├── predict_test.py # Tests model predictions
│
├── models/
│ ├── emotion_model.h5 # Emotion prediction model
│ ├── intensity_model.h5 # Intensity prediction model
│
├── preprocessing_objects.pkl # Contains scalers/encoders for preprocessing
│
├── app.py # Flask application entry point
│
├── templates/
│ └── index.html # Web UI (input + result display)
│
├── static/
│ ├── index.css # CSS for the web app
│ └── background.png # Background image
│
├── requirements.txt # Project dependencies
│
└── README.md # Project documentation


---

## ⚙️ Installation

### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/EEG_Emotion_Recognition.git
cd EEG_Emotion_Recognition

Step 2: Create a Virtual Environment
python -m venv venv
venv\Scripts\activate      # For Windows
# or
source venv/bin/activate   # For macOS/Linux

Step 3: Install Dependencies
pip install -r requirements.txt

🧠 Usage
1️⃣ Preprocess the Data
python preprocess.py


This script cleans and prepares EEG data for training.

2️⃣ Train the Model
python train_model.py


Trains and saves the emotion and intensity models.

3️⃣ Test the Model
python predict_test.py


Loads the trained models and verifies predictions.

4️⃣ Run the Flask Web App
python app.py


Open your browser and go to:

http://127.0.0.1:5000

🌐 Web Interface

Click “Test it” to open the input form

Enter EEG values: Attention, Meditation, Eye Blink, Average

Click “Find Your Emotion” to get predictions

You’ll see the Predicted Emotion and Predicted Intensity displayed on the same page.

🧾 Example Output
Attention	Meditation	Eye Blink	Average	Predicted Emotion	Intensity
0.72	0.60	0.12	0.48	Happy	0.82
🌱 Future Enhancements

Integration with real-time EEG hardware (e.g., MindWave headset)

Model optimization using hybrid CNN-LSTM architecture

Deployment on Render, AWS, or Azure for live demos

Add emotion visualizations using Chart.js

📸 Screenshots (Optional)

You can include these if you want later:

static/background.png
templates/index.html

📄 License

This project is open-source and available for educational and research purposes.
