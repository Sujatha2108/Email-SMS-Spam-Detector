# 📧 Email & SMS Spam Detector

A simple web application to classify text as "Spam" or "Ham" (not spam). This project uses a fine-tuned **DistilBERT** model from **Hugging Face Transformers**, served with a lightweight **Flask** app.

The entire project, from data exploration and model training to final deployment, is contained within a single Google Colab notebook.

## ✨ Features

* **Real-time Prediction:** Instantly classifies any input text as "Spam" or "Ham."
* **Confidence Score:** Shows the model's confidence percentage in its prediction.
* **Interactive UI:** A clean and simple web form built with Flask and HTML.
* **All-in-One Notebook:** The Google Colab notebook contains:
    * Data loading and preprocessing.
    * Fine-tuning the `DistilBERT` model on a spam dataset.
    * Pushing the final model to the Hugging Face Hub.
    * The complete Flask application code.
    * One-click deployment using `pyngrok`.

## 🛠️ Technology Used

* **Python 3**
* **Google Colab** (for development and training)
* **Hugging Face `transformers`** (for the `DistilBERT` model and `pipeline`)
* **Hugging Face `datasets`** (for loading data)
* **PyTorch** (as the backend for Transformers)
* **Flask** (for the web server)
* **pyngrok** (for tunneling and public deployment from Colab)
* **Pandas** (for data manipulation)
* **Scikit-learn** (for evaluation metrics)
