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

## ▶️ 4. How to Run the Project  

### **Step 1 → Google Colab Setup**
Create a Colab notebook.

### **Step 2 → Upload Dataset**
Path required:  
