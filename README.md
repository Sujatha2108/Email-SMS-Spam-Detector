# 📧 Email & SMS Spam Detector

A simple web application to classify text as "Spam" or "Ham" (not spam). This project uses a fine-tuned **DistilBERT** model from **Hugging Face Transformers**, served with a lightweight **Flask** app.

The entire project, from data exploration and model training to final deployment, is contained within a single Google Colab notebook.

## 🚀 Demo

Here is the final application in action, deployed directly from Google Colab using `pyngrok`:

*(**Note:** This is the most important part of your README! Create a short GIF from your `Email_Spam.mp4` video and drag-and-drop it here. You can use a free online tool like [ezgif.com]("C:\Users\SUJATHA ALUGOJU\Videos\Captures\Email_Spam - Colab - Google Chrome 2025-10-24 19-13-18.mp4") to convert your MP4 to a GIF.)*

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

## 🏃 How to Run

The easiest way to get started is to run the project directly in Google Colab.

1.  **Open the Notebook:**
    * Go to [Google Colab](https://colab.research.google.com/).
    * Upload the `Email_Spam.ipynb` file from this repository (`File` > `Upload notebook...`).

2.  **Set Runtime:**
    * In the Colab menu, go to `Runtime` -> `Change runtime type`.
    * Select **GPU** as the hardware accelerator. This will make model training and inference significantly faster.

3.  **Run the Cells:**
    * Run all the cells in the notebook from top to bottom (`Runtime` > `Run all`).
    * The notebook will install all required libraries, load the data, fine-tune the model, and finally, define and start the Flask app.

4.  **Access the App:**
    * The very last cell will execute `pyngrok` and print a public URL.
    * It will look something like `https://<some-random-string>.ngrok.io`.
    * Click this URL to open the live application in your browser and test it!

## 🤖 About the Model

This project uses `distilbert-base-uncased`, a smaller, faster, and lighter version of the BERT model, which makes it ideal for web applications.

It was fine-tuned on a public SMS/Email Spam dataset to specialize it for this classification task. The fine-tuning process adapts the general-purpose language model to become a highly accurate spam detector.

The final trained model is also available on the Hugging Face Hub:
**[Link to your Hugging Face Model Hub repo]**

*(**Note:** Remember to push your model to the Hub (as shown in your video) and paste the link here! Example: `https://huggingface.co/SujathaAlugoju/distilbert-spam-detector`)*

## License

This project is open-source and available under the [MIT License](LICENSE).
