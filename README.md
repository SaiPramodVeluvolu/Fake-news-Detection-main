=======
App still on development
>>>>>>> 118f055b82567e698f5892e1ca8eb0a0e393c5f1

```markdown
# Fake News Detection Project

This project demonstrates a fake news detection pipeline using various NLP techniques and machine learning frameworks. Built with Python, it incorporates traditional machine learning approaches as well as deep learning models using BERT embeddings.

## Features

- **Data Handling & Preprocessing:**
  - Uses `pandas` and `numpy` to manage datasets.
  - Text cleaning using Python's `re` module.
  - Tokenization, stopword removal, and lemmatization using `nltk` and `spaCy`.

- **Machine Learning Pipelines:**
  - **Random Forest Classifier** and **XGBoost** for fake news classification.
  - **BERT-based model** for generating embeddings and performing classification.

- **Deployment:**
  - Flask web app interface to predict fake news interactively via a simple HTML form.

- **Model Evaluation:**
  - Models are evaluated using accuracy, confusion matrices, and other metrics.

## Project Structure

```bash
fake_news_detection/
├── App/
│   └── templates/
│       └── index.html       # Front-end HTML template
│   └── app.py               # Flask app for serving predictions
├── Data/
│   └── Dataset/
│       └── data.csv         # Training dataset with news text and labels
├── Models/
│   ├── model.pkl            # Main trained model
│   ├── random_forest.pkl    # Random Forest model
│   ├── xgboost_model.pkl 
├── Notebooks/
│   └── Fakenewsdetection.ipynb # Experimenting and testing modules
├── Main.py                  # Script for training and evaluating models
├── app.py                   # Flask app
├── README.md                # This file
├── requirements.txt         # Project dependencies
```

## Setup and Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/fake-news-detection.git
   cd fake-news-detection
   ```

2. **Create and Activate a Virtual Environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate   # For Unix/Linux
   venv\Scripts\activate      # For Windows
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Download spaCy Model:**

   ```bash
   python -m spacy download en_core_web_sm
   ```

## Running the Project

### Training the Models

Run the script to preprocess the data, train models, and evaluate performance:

```bash
python Main.py
```

### Running the Web App

Start the Flask app to interactively classify news text:

```bash
python app.py
```

Open your browser and go to `http://127.0.0.1:5000/` to use the Fake News Detector.

## Additional Information

- **Model Pipelines:** This project includes multiple model pipelines, including traditional machine learning, gradient boosting, and deep learning using BERT embeddings.
- **Web Interface:** The Flask web app allows users to submit text and receive predictions about whether the news is real or fake.
- **Experiments:** Jupyter notebooks are included for experimenting with different preprocessing techniques and model architectures.

## Acknowledgements

- Libraries: `nltk`, `spaCy`, `transformers`, `scikit-learn`, `xgboost`, `tensorflow`
- Models: Pre-trained BERT from Hugging Face
```

#   F a k e - N e w s - D e t e c t i o n - N L P  
 