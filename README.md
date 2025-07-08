## 📌 Overview
This project applies a **linear Support Vector Machine (SVM)** to the SMS Spam Collection dataset to build a simple, interpretable spam filter. It shows how a classic algorithm can perform well on real-world text data with minimal tuning.

## 📊 Dataset
- **Name**: SMS Spam Collection  
- **Records**: 5,574 SMS messages labeled as `spam` or `ham` (not spam)  
- **Features**: Raw message text, transformed using TF-IDF (~3,964 features)  

## ⚙️ Preprocessing
- Loaded raw text messages
- Converted messages into numerical features using TF-IDF vectorization
- Removed English stop words
- Encoded labels (`ham` → 0, `spam` → 1)


## 🧠 Model Training
- **Model**: `SVC(kernel='linear', C=1)`
- **Tuning**: GridSearchCV over `C` values
- **Split**: 85% training, 15% testing


## ✅ Results
- **Accuracy**: 98.5%  
- **Recall (Spam)**: 91%  
- No class weighting needed — the linear model performed well as-is.


## 🙋‍♂️ Author
Adewunmi Jesusegun 
Part of the **“One Model. One Project.”** series documenting hands-on ML work with one model at a time.

