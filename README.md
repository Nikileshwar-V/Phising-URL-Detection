# Phishing URL Detection Using Machine Learning

This project focuses on detecting phishing URLs using machine learning techniques, particularly a Random Forest Classifier. The aim is to build a reliable model to classify URLs as either phishing or legitimate, using a set of extracted features.

## 📦 Repository Contents

```
Phishing-URL-Detection/
│
├── urldataset.csv               # Dataset containing URLs and their features
├── phishing_rf_model.pkl        # Saved trained Random Forest model
├── phishing_url_detection.ipynb # Google Colab notebook for feature extraction, model training, and prediction
└── README.md                    # Project documentation
```

---

## 🔍 Project Overview

Phishing is a common cybersecurity threat that uses fake URLs to deceive users into revealing sensitive information. This project aims to:

✅ Extract meaningful features from URLs (like domain length, HTTPS usage, and special character ratios).
✅ Train a Random Forest Classifier using these features to distinguish between phishing and legitimate URLs.
✅ Save the trained model for easy reuse.
✅ Provide a **Google Colab notebook** that integrates feature extraction, model training, and prediction in one place.

---

## 📁 Dataset

* **File**: `urldataset.csv`
* **Columns**:

  * `FILENAME`, `URL`, `URLLength`, `Domain`, `DomainLength`, `IsDomainIP`, `TLD`, `URLSimilarityIndex`, `CharContinuationRate`, `TLDLegitimateProb`, `URLCharProb`, `TLDLength`, `NoOfSubDomain`, `HasObfuscation`, `NoOfObfuscatedChar`, `ObfuscationRatio`, `NoOfLettersInURL`, `LetterRatioInURL`, `NoOfDegitsInURL`, `DegitRatioInURL`, `NoOfEqualsInURL`, `NoOfQMarkInURL`, `NoOfAmpersandInURL`, `NoOfOtherSpecialCharsInURL`, `SpacialCharRatioInURL`, `IsHTTPS`, `LineOfCode`, `LargestLineLength`, `HasTitle`, `Title`, `DomainTitleMatchScore`, `URLTitleMatchScore`, `HasFavicon`, `Robots`, `IsResponsive`, `NoOfURLRedirect`, `NoOfSelfRedirect`, `HasDescription`, `NoOfPopup`, `NoOfiFrame`, `HasExternalFormSubmit`, `HasSocialNet`, `HasSubmitButton`, `HasHiddenFields`, `HasPasswordField`, `Bank`, `Pay`, `Crypto`, `HasCopyrightInfo`, `NoOfImage`, `NoOfCSS`, `NoOfJS`, `NoOfSelfRef`, `NoOfEmptyRef`, `NoOfExternalRef`, `label`
* **Label**:

  * `0` for legitimate URLs
  * `1` for phishing URLs

---

## 🔨 How to Use

### 1️⃣ Open the Notebook

* Launch the `phishing_url_detection.ipynb` notebook in Google Colab.

### 2️⃣ Load the Dataset

* The notebook reads `urldataset.csv` and processes all features.
* Make sure `urldataset.csv` is uploaded to your Colab environment.

### 3️⃣ Train the Model

* The notebook uses the dataset to train a Random Forest Classifier on all relevant features.
* The trained model is saved as `phishing_rf_model.pkl` for reuse.

### 4️⃣ Make Predictions

* You can use the notebook’s prediction cells to classify any URL as phishing or legitimate.
* Features are extracted automatically from the input URL to match the trained model’s expectations.

---

## 🧩 Key Features

✅ **55 Features Extracted**
Including URL length, special character counts, domain features, HTTPS presence, and more.

✅ **Model Training and Evaluation**
Random Forest Classifier is trained with robust validation.

✅ **Model Saving**
The trained model is saved as `phishing_rf_model.pkl` using Pickle.

✅ **Colab Friendly**
All tasks—feature extraction, model training, saving, and prediction—are done inside one notebook, making it easy to reproduce and understand.

---

## 📌 Notes

* The notebook uses preprocessed features. If using new URLs, ensure that feature extraction is consistent.
* The saved model (`phishing_rf_model.pkl`) can be reloaded and used to predict phishing URLs.
* This setup does not include a web interface, focusing solely on the machine learning pipeline.

---

## 💡 Future Enhancements

* Add a user-friendly web interface using Flask or Streamlit (optional).
* Incorporate deep learning models for further accuracy improvements.
* Extend feature extraction to include lexical and contextual analysis of URLs.

---

## 🤝 Contributions

Contributions and feedback are welcome! Feel free to open an issue or submit a pull request.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

Thanks to the cybersecurity and data science communities for inspiration and resources.

---
**Author**
NIKILESHWAR.V MCA Student | AI/ML Enthusiast | Open to Internships & Collaboration 📫 Connect with me: https://www.linkedin.com/in/nikileshwarv/
********** Phising-URL-Detection ***********
