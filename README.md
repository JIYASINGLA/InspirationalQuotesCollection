# Inspirational Quotes Collection  
### Analyzing Positive & Inspirational Language in Large Quote Datasets

## 📝 1. Problem Statement  
Inspirational and motivational quotes often use uplifting words such as **hope, dream, success, courage** and more.  
However, without automated analysis, we cannot identify:

- Which motivational words appear most frequently  
- What themes dominate across thousands of quotes  
- How quotes behave under custom NLP rule-based detectors  

This project analyzes **1000–2000 inspirational quotes** to uncover:

- The most common positive words  
- Repeated themes such as hope, struggle, wisdom, emotion, action  
- NLP-based rule detections  
- Visual patterns through charts  

---

## 🎯 2. Project Objectives  

### **Main Objectives**
- Clean and preprocess a large inspirational text dataset  
- Count the frequency of powerful motivational words:
  - success, dream, believe, hope, courage  
  - future, goal, trust, achieve  
- Apply **8 rule-based NLP detectors**
  - Positive words  
  - Hope + struggle  
  - Long quotes  
  - Emotional words  
  - Wisdom words  
  - Action words  
  - Negation  
  - Questions  

### **What You Will Learn**
- Text preprocessing  
- Regex-based rule design  
- Word frequency analysis  
- Multithreading with ThreadPoolExecutor  
- Matplotlib visualizations  
- Saving data into CSV + SQLite  

---

## 🔄 3. Workflow Overview  

### **Step 1 → Import Libraries**
Using:
- pandas  
- re  
- matplotlib  
- concurrent.futures  
- sqlite3  

### **Step 2 → Load Dataset**
Reads: `inspirational_quotes.txt`

### **Step 3 → Clean Text**
- Lowercase  
- Remove punctuation  
- Keep only clean word tokens  

### **Step 4 → Chunking**
Break quotes into chunks for multithreading.

### **Step 5 → Parallel Word Counting**
Counts motivational words using ThreadPoolExecutor.

### **Step 6 → Apply 8 NLP Rules**
Detect:
- Positive words  
- Hope + struggle  
- Long quotes  
- Emotional words  
- Wisdom  
- Action verbs  
- Negation  
- Questions  

### **Step 7 → Save Results**
Outputs:
- `results_inspirational_quotes.csv`
- `results_inspirational_quotes.db`
- `rule_plan.csv`

### **Step 8 → Visualize Data**
- Bar Chart  
- Pie Chart  

---

---

## ▶️ 4. How to Run the Project (Step-by-Step)

### **1. Download the Dataset**
- Download or prepare the file: `inspirational_quotes.txt`
- Upload it to Google Drive at:
- /content/drive/MyDrive/NLP_project/
- 
### **2. Open Google Colab**
- Go to https://colab.research.google.com/
- Create a new Python Notebook.

### **3. Mount Google Drive**
Run:
```python
from google.colab import drive
drive.mount('/content/drive')

**### **4. Add the Python Script****

-Paste your full project code into the Colab notebook.
-Ensure file paths are set correctly:
-FILE_PATH = '/content/drive/MyDrive/NLP_project/inspirational_quotes.txt'
-CSV_OUTPUT = '/content/drive/MyDrive/NLP_project/results_inspirational_quotes.csv'
-DB_OUTPUT = '/content/drive/MyDrive/NLP_project/results_inspirational_quotes.db'
-RULE_PLAN_CSV = '/content/drive/MyDrive/NLP_project/rule_plan.csv'

**### 5. Run the Main Function**

-Execute:
-main()
