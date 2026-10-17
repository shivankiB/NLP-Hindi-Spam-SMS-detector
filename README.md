# Hindi-Spam-SMS-detector

## 📁 Project Structure and instructions
- NlpProj.ipynb` -> The Google Colab notebook containing code.
- hindi_sms_dataset_extended.csv` -> Text dataset.
- hindi_stopwords.txt -> Stopwords dataset.
- Download the colab book and run the codes to train and save the models

### Model Evaluation & Sample Predictions

Below is a demonstration of how different feature extraction techniques perform on a sample Hindi text input using an SVM (Support Vector Machine) classifier.

### Test Case Example

Input Hindi Text:
"बैंक" और "विशेष ऑफर" विश्वसनीय लगते हैं, लेकिन यह स्पैम या प्रचार हो सकता है।
(Translation: "Bank" and "Special Offer" sound trustworthy, but this could be spam or promotion.)

### 📊 Classifier Results Comparison

<img width="1142" height="140" alt="image" src="https://github.com/user-attachments/assets/bae3f153-226c-4c1c-82ea-b3bba757c645" />


Bag of Words (BoW)	['ham']	✅ Correct

TF-IDF	['ham']	✅ Correct

FastText Embeddings	['ham']	✅ Correct

Combined Features (Ensemble/Hybrid)	['spam']	❌ Misclassified


### 💡 Key Takeaway

This example highlights a classic edge case in text classification. While the text contains strong spam signals or keywords (like "विशेष ऑफर" and "स्पैम"), the sentence structure is actually informative (ham). The individual models successfully captured this nuance, whereas the Combined Features model over-relied on keyword density, resulting in a false-positive spam prediction.
