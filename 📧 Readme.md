# 📧 Email Spam Classification

A machine learning web application that classifies messages as **Spam** or **Ham (Not Spam)**.

The project uses **Natural Language Processing (NLP)** techniques and a **Bernoulli Naive Bayes** machine learning model to predict whether a given message is spam.

## 🚀 Features

- Classifies messages as **Spam** or **Ham**
- Uses **Bag of Words** for text vectorization
- Uses **Bernoulli Naive Bayes** for classification
- Simple web interface built with Flask
- Pre-trained machine learning model
- Easy to run locally

## 🛠️ Technologies Used

- Python
- Flask
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Joblib

## 📂 Project Structure

```text
Email_classification/
│
├── models/
│   ├── bag_of_words.lb
│   └── bernouliNB.lb
│
├── templates/
│   ├── index.html
│   └── output.html
│
├── SMSSpamCollection.txt
├── email.ipynb
├── app.py
├── requirment.txt
└── README.md
```

## 🧠 How It Works

The application follows these steps:

1. The user enters a message in the web interface.
2. The message is converted into numerical features using a **Bag of Words** model.
3. The transformed message is passed to the trained **Bernoulli Naive Bayes** classifier.
4. The model predicts the message as:

   - `0` → **Ham**
   - `1` → **Spam**

5. The prediction is displayed on the web page.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/SoyalIslam/Email_classification.git
```

### 2. Navigate to the project directory

```bash
cd Email_classification
```

### 3. Create a virtual environment

```bash
python -m venv email
```

### 4. Activate the virtual environment

#### Windows

```bash
email\Scripts\activate
```

#### Linux / macOS

```bash
source email/bin/activate
```

### 5. Install the required dependencies

```bash
pip install -r requirment.txt
```

## ▶️ Run the Application

Run the Flask application using:

```bash
python app.py
```

After running the application, open your browser and visit:

```text
http://127.0.0.1:5000/
```

## 🖥️ Usage

1. Open the application in your browser.
2. Enter a message or email text.
3. Submit the message.
4. The application will predict whether the message is:

```text
Spam 🚨
```

or

```text
Ham ✅
```

## 📊 Machine Learning Model

The project uses:

### Bag of Words

The text messages are converted into numerical features using the **Bag of Words** technique.

### Bernoulli Naive Bayes

The **Bernoulli Naive Bayes** algorithm is used to classify messages into Spam or Ham categories.

The trained model and vectorizer are stored inside the `models/` directory and loaded using `joblib`.

## 📁 Dataset

The project uses the `SMSSpamCollection.txt` dataset for training and testing the spam classification model.

The dataset contains labeled messages categorized as:

- **Ham** – legitimate messages
- **Spam** – unwanted or promotional messages

## 🔮 Future Improvements

- Add prediction probability/confidence
- Improve the user interface
- Add more advanced NLP preprocessing
- Compare multiple machine learning models
- Deploy the application online
- Add support for full email classification

## 👨‍💻 Author

**Soyal Islam**

## 📜 License

This project is created for learning and educational purposes.
