# Hindi-Spam-SMS-detector

🔮 Model Evaluation & Sample Predictions

Below is a demonstration of how different feature extraction techniques perform on a sample Hindi text input using an SVM (Support Vector Machine) classifier.

Test Case Example

Input Hindi Text:
"बैंक" और "विशेष ऑफर" विश्वसनीय लगते हैं, लेकिन यह स्पैम या प्रचार हो सकता है।
(Translation: "Bank" and "Special Offer" sound trustworthy, but this could be spam or promotion.)

📊 Classifier Results Comparison

<img width="1142" height="140" alt="image" src="https://github.com/user-attachments/assets/bae3f153-226c-4c1c-82ea-b3bba757c645" />


Feature Extraction Method	Prediction Outcome	Status
Bag of Words (BoW)	['ham']	✅ Correct
TF-IDF	['ham']	✅ Correct
FastText Embeddings	['ham']	✅ Correct
Combined Features (Ensemble/Hybrid)	['spam']	❌ Misclassified


💡 Key Takeaway

While individual semantic or frequency-based feature extraction models (like BoW, TF-IDF, and FastText) failed to flag the deceptive nature of the text on their own, the Combined Features approach successfully caught the subtle patterns to accurately classify it as spam.
