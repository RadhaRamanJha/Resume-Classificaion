# Resume Classification

## 🔍 Business Objective  
The goal of this project is to reduce manual human effort in the recruitment process by automatically classifying resumes into predefined categories using Natural Language Processing (NLP) and Machine Learning techniques.

---

## 📂 Project Overview  

### 1. Data Gathering  
- All resumes (PDF/DOC) were converted to `.docx` using `pdf2docx` and `doc2docx` libraries.  
- `textract` was used to extract text from `.docx` files.  
- Resumes were categorized into Internship, ReactJS, PeopleSoft, SQL, and Workday.  
- All data was combined into a single DataFrame and labeled using `LabelEncoder`.  
- Saved as `resume_data.csv` for further processing.

### 2. Data Cleaning  
- Removed whitespace, converted text to lowercase, and performed tokenization.  
- Applied stemming and lemmatization.  
- Removed stop words (e.g., “is”, “are”, “we”).  
- Performed Part-of-Speech tagging.  
- Cleaned data stored separately as `clean_resumes.csv`.

### 3. Exploratory Data Analysis (EDA)  
- TF-IDF analysis was conducted.  
- Word frequency plots and n-gram (bi/tri-gram) visualizations created for each category.  
- Word clouds generated to highlight key terms by category.

### 4. Model Building  
Dataset was split: 75% training / 25% testing  
Applied classifiers:  
- K-Nearest Neighbors (KNN)  
- Decision Tree  
- Random Forest  
- Support Vector Machine (SVM)  
- Bagging Classifier  
- AdaBoost  
- Naive Bayes  

### 5. Model Evaluation  
Metrics considered:  
- Training Accuracy  
- Testing Accuracy  
- Precision  
- Recall  
- F1-Score  

Bar charts and tables were used to compare model performance.

---

## 🚀 Deployment  
The best-performing model was deployed using **Streamlit** for an interactive resume classification interface.

---

## 📁 Files Included  
- `Clean_resumes.csv`, `resume_data.csv` – Preprocessed datasets  
- `EDA.ipynb` – EDA notebook  
- `Model_Building_Final.ipynb` – Final model training  
- `classification_model.ipynb` – Alternate model trial  
- `VECTOR.pkl`, `ModelDTC.pkl` – Saved vectorizer & model  
- `Resume_app1.py` – Streamlit app for deployment  
- `Project - Resume Classification.pptx` – Presentation  
- `README.md` – Project documentation

---

## 🔗 Author  
[Radha Raman Jha](https://www.linkedin.com/in/radha-raman-jha-a565a2102)  
[GitHub Repository](https://github.com/RadhaRamanJha/Resume-Classificaion)
