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


## 🔄 3. How the Code Works (Workflow Overview)

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


## 🚀 4. How to Run the Project

**Step 1: Open Google Colab**  
https://colab.research.google.com

**Step 2: Click on:** File → Open Notebook  

**Step 3: Go to the GitHub tab**  

Paste your GitHub repository link  
(the one where your `.ipynb` file is uploaded)  

**Step 4: Select the notebook file → Open it**  

**Step 5: Once the notebook loads, click:** Runtime → Run all  

Wait for all cells to complete.  

The project will:  
- load the quotes dataset  
- preprocess text  
- apply NLP rules  
- perform parallel processing  
- generate word frequency results  
- create charts  
- save CSV + database files  

Your output (CSV, charts, database) will appear in Colab after execution.


## 🧠 5. Rule-Based Detection System

| Rule Name              | Purpose                               |
|------------------------|----------------------------------------|
| Positive Word Detector | Finds motivational keywords            |
| Hope + Struggle        | Detects quotes mixing hope & struggle  |
| Long Quote             | Finds quotes > 20 words                |
| Action Word            | Detects action verbs (start, act, rise)|
| Emotion Word           | Detects emotional words (love, joy, care) |
| Wisdom Word            | Detects wisdom-based words (learn, teach, understand) |
| Negation               | Detects negation (not, never, don’t)   |
| Question Detector      | Detects the presence of “?”            |


## 📊 6. Expected Output

#### **CSV Example**
Displays the word-frequency output generated after analysis.

<img width="1377" height="847" alt="CSV Example" src="https://github.com/user-attachments/assets/bf8dee61-a061-4438-9c2b-6068e01cbd52" />


#### **Bar Chart**
Shows the frequency of selected positive words.

<img width="1961" height="683" alt="Bar Chart" src="https://github.com/user-attachments/assets/9fa0972d-b9db-43e6-b8e6-e00bd8ff9312" />


#### **Pie Chart**
Represents the percentage contribution of each positive word.

<img width="1460" height="990" alt="Pie Chart" src="https://github.com/user-attachments/assets/17ab40a6-f13d-4b98-863e-e0ed8b07e153" />


## 🔮 7. Future Scope

This project can be expanded and improved in several ways:

- **Add More Data Sources:**  
  Integrate APIs (Quotes API, Goodreads scraping, etc.) to collect 10,000+ quotes automatically.

- **Advanced NLP Techniques:**  
  Use NLP libraries like **NLTK, spaCy, or transformers** to perform:
  - Sentiment analysis  
  - Topic modeling  
  - Named entity recognition  

- **Interactive Dashboard:**  
  Build a web-based dashboard using **Streamlit or Plotly Dash** to visualize frequencies and rule-based detections in real time.

- **Multi-Language Support:**  
  Analyze inspirational quotes in Hindi, Punjabi, Spanish, etc., to compare motivational themes across cultures.


## 🏁 8. Conclusion

This project offers strong practical knowledge in:

- **Text cleaning & NLP preprocessing**
- **Rule-based NLP design**
- **Word frequency modeling**
- **Data visualization using Matplotlib**
- **CSV and SQLite database storage**

It successfully identifies dominant motivational themes within inspirational literature and builds real-world NLP skills using **Python, Regex, ThreadPoolExecutor, and Matplotlib**.

