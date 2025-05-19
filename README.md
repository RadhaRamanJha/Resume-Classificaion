# Resume-Classificaion
## Business objective

### The document classification aims to reduce the manual human effort in the HRM. It aims to achieve a higher level of accuracy and automation with minimal human intervention

# Project Description 
**1. Data Gathering**
1.	All pdf and doc file are coverted to .docx file type using pdf2docx.Convert and doc2docx.convert methods of respective libaries
2.  All resumes of .docx extension is converted to text using textract module of pandas to bring it in a DataFrame eventually
3.	Data frame for every resume categories i.e. Internship, ReactJS, PeopleSoft, SQL and Workday were built
4.	All the DataFrame was combined as single DataFrame using DataFrame.append()  
5.	Using the label encoder a sperate numerals is assigned for each resume category
6.	Saved the DataFrame as csv file to proceed with Data Peprocessing


**2. Data Cleaning**
1. Dataset still has a huge number of records was still very rough and unclassified.
2. Data cleaning was done by removing any blank spaces from the data, then changing all the text to lowercase followed by tokenization.
3. Stemming and Lemmatization (reducing the word to it's root words) to avoid confusion and removing stop words from the data.
   - Stop words are those words which don’t play an important role in sentence formation, such as “are”, “we”, “is”, etc.
4. Next the part-of-speech tagging of the words was done
   
![image](https://github.com/user-attachments/assets/c1616ddf-399d-4b20-b1b3-b3163c7a806e)

5. Cleaned data was stored as a separate dataset.
   
**3. Exploratory Data Analysis**
1. The Term frequency and Inverse document frequencies of each word present in resume was identified
2. Created single word frequency plot.

![image](https://github.com/user-attachments/assets/c254abe1-647a-40cb-9b14-bfc70eee747c)

3. Created bigrams (2 words at a time) and trigrams(3 words at a time) for cleaned format of resume for all the categories
e.g. :-
PeopleSofy resumes :- 

![image](https://github.com/user-attachments/assets/c68c3681-1b01-4a48-ae33-f4009c7f24d8)

ReactJs resumes :- 

![image](https://github.com/user-attachments/assets/27b463dd-b8a5-4526-b3a7-5f89791e5c5d)


6. Created world cloud plot for each category of resume for better visual identification of important words


![image](https://github.com/user-attachments/assets/8bfa7a1a-c5e9-4c3a-8efe-26fbf1d66336)


**4. Model Traning and application of classification alogrithms to the databasets**
1. The dataset was partitioned in 75% trainging dataset and 25% testing dataset
2. Models were prepared using several classifiers
   - KNN classifier

![image](https://github.com/user-attachments/assets/b3f6c009-b1d5-40cc-a786-7820d67f4e47)

   - Decision Tree Classifier

![image](https://github.com/user-attachments/assets/d172b401-8b1d-43a7-9df8-f9e34a8968b3)

   - Random Forest Classifier

![image](https://github.com/user-attachments/assets/c5ed1064-ee72-43b5-a216-00a3ae7b562e)

   - SVM classifier

![image](https://github.com/user-attachments/assets/33076cf8-77b6-434a-a5dc-49cef831ae4b)

   - Bagging classifier

![image](https://github.com/user-attachments/assets/b1493f77-b351-479f-9e66-39ce1d87102e)

   - Ada boost classifer

![image](https://github.com/user-attachments/assets/40061e01-caec-4759-bd4e-463f0c6ea716)

   - and Naive Bayes Classifier

![image](https://github.com/user-attachments/assets/f308ba13-677f-421d-9dc0-2bd4ab7a92a8)


**5. Model Evaluation**
1. All the models are tabulated for the comparision in terms of
   - Trainig accuracy
   - Testing accuracy
   - Precision
   - Recall
   - F1-score
  

  ![image](https://github.com/user-attachments/assets/9a7bd3dd-7db9-4337-87f9-a7a7b3242676)

Bar Chart representing the accuracy of Training data as well as Testing data

![image](https://github.com/user-attachments/assets/6f51bf2b-7bd5-467b-8eeb-e347248df536)

Finally the Model was deployed using streamlit
