# Resume-Classificaion
## Business objective

### The document classification aims to reduce the manual human effort in the HRM. It aims to achieve a higher level of accuracy and automation with minimal human intervention

# Project Description 
**1. Data Extraction from all resumes in form of CSV file**
1.	All pdf and doc file are coverted to .docx file type using pdf2docx.Convert and doc2docx.convert methods of respective libaries
2.  All resumes of .docx extension is converted to text using textract library to bring it in a DataFrame eventually
3.	Data frame for every resume categories i.e. Internship, ReactJS, PeopleSoft, SQL and Workday were built
4.	All the DataFrame was combined as single DataFrame using DataFrame.append()  
5.	Using the label encoder a sperate numerals is assigned for each resume category
6.	Saved the DataFrame as csv file to proceed with Data Peprocessing

