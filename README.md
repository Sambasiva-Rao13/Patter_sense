# 🧵 Pattern Sense: Classifying Fabric Patterns using Deep Learning

**Pattern Sense** is a deep learning project that classifies fabric patterns such as floral, plain, ikat, and more using a trained Convolutional Neural Network (CNN). It is integrated with a Flask-based web interface that allows users to upload an image and instantly see the predicted fabric pattern.

---

## 🚀 Demo

https://drive.google.com/file/d/1-StquWipy3ODTNxAXpfUbrTjzx2WLWMi/view?usp=sharing

---

## 🧠 Technologies Used

- **Python 3.x**
- **TensorFlow & Keras** – Deep Learning Framework
- **Flask** – Web Framework
- **OpenCV & Pillow** – Image processing
- **HTML5, CSS3** – Frontend Interface
- **Jinja2** – HTML templating in Flask

---

## 📁 Project Structure

Pattern_Sense_Project/
├── app.py # Flask application
├── train_model.py # Script to train and save the model
├── model/
│ └── model_cnn (2).h5 # Trained CNN model file
├── dataset/ # Fabric images in class subfolders
│ ├── floral/
│ ├── plain/
│ └── ikat/
├── templates/
│ ├── home.html # Homepage
│ ├── predict.html # Image upload and preview
│ └── predictionpage.html # Display prediction result

---

## 🎯 Features

- 🔍 Real-time fabric pattern recognition
- 🧠 Trained CNN model with high accuracy
- 🌐 Flask-based local web application
- 🖼️ Live preview of uploaded images
- 📂 Easily extendable dataset structure
- 💡 Simple, responsive UI

---

## 🧪 Dataset Structure

To train the model, the dataset must be structured like this:
dataset/
├── floral/
│ ├── image1.jpg
│ ├── image2.jpg
│ └── ...
├── plain/
│ └── ...
├── ikat/
│ └── ...


Each subfolder represents a fabric pattern class. The more images per class, the better the model's performance.

---

## 🏗️ Model Overview

- **Model Type:** CNN (Convolutional Neural Network)
- **Layers:** Conv2D → MaxPooling → Flatten → Dense
- **Output Activation:** Softmax
- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Accuracy Achieved:** ~90% on validation data (varies by dataset)

The trained model is saved as:  
`model/model_cnn (2).h5`

---

## ⚙️ How to Run the Project

### ✅ Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/Pattern_Sense_Project.git
cd Pattern_Sense_Project
```

###✅ Step 2: Create Virtual Environment (Optional but Recommended)
bash
Copy
Edit
python -m venv venv
# Activate it:
# On Windows:
venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate

###✅ Step 3: Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt

###✅ Step 4: Run the Flask App
bash
Copy
Edit
python app.py

###✅ Step 5: Open in Browser
Visit http://127.0.0.1:5000 to access the application.

🖼️ How It Works
Upload a fabric image using the web interface.

The image is preprocessed and passed to the trained CNN model.

The predicted fabric class is displayed on a new page.

📄 requirements.txt (if needed)
txt
Copy
Edit
flask
tensorflow
numpy
pillow
opencv-python
Generate it using:

bash
Copy
Edit
pip freeze > requirements.txt

📌 Created by: Chattu Samba Siva Rao
Computer Science & Engineering(Artificial Intelligence and Machine Learning) | Ideal Institute of Technology | JNTU Kakinada
Pattern Sense – 2025 AI-ML Mini Project

