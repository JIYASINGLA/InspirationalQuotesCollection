**Motivational Word Frequency Analyzer**
Analyzing Positive & Inspirational Language in Large Quote Datasets

**1. Problem Statement**

Inspirational and motivational quotes often use emotionally uplifting words such as hope, dream, success, and courage. However, without analysis, we do not know which motivational words appear most frequently across thousands of quotes.

The goal of this project is to analyze a large dataset of inspirational quotes (1000–2000 lines) and identify:

Which positive or motivational words occur most often

What themes (hope, struggle, emotion, wisdom, action) appear repeatedly

How quotes behave under custom NLP rule-based detectors

This project helps uncover linguistic patterns, emotional tone, and common motivational themes used in modern inspirational literature.

**2. Project Objectives**
**Main Objectives**

Extract and clean a large dataset of inspirational text.

Count the frequency of selected positive/motivational words:
success, dream, believe, hope, courage, future, goal, trust, achieve

Apply 8 NLP rule-based detectors:

Positive words

Hope + struggle

Long quotes

Emotional words

Wisdom words

Action words

Negation words

Question detector

**What You Will Learn**

Text preprocessing (cleaning, tokenizing)

Word frequency analysis

Parallel processing using ThreadPoolExecutor

Creating data visualizations with Matplotlib

Designing custom NLP rules using regex

Saving data to CSV and SQLite database

**3. How the Code Works (Workflow Overview)**
**Step 1 → Import Libraries**

pandas

re (regex)

matplotlib

concurrent.futures

sqlite3

**Step 2 → Load Dataset**

Reads the .txt file containing 1000–2000 quotes.

**Step 3 → Clean Text**

Convert to lowercase

Remove punctuation

Keep only words and “?” for question rule

**Step 4 → Chunking**

Breaks text into chunks of 20 lines for multithreading.

**Step 5 → Parallel Word Counting**

Counts occurrences of every positive word using ThreadPoolExecutor.

**Step 6 → Apply 8 NLP Rules**

Rules detect:

Positive words

Hope + struggle combinations

Long quotes

Emotional words

Wisdom words

Action verbs

Negation

Questions

**Step 7 → Save Results**

Outputs include:

CSV file

SQLite database

Rule plan CSV

Console print of matched rules

**Step 8 → Visualize Data**

Bar chart

Pie chart

**4. How to Run the Project (Step-by-Step)**
**Step 1: Setup in Google Colab**

Open Google Colab.

Create a new Python notebook.

**Step 2: Upload Dataset to Google Drive**

Place this file inside:

/content/drive/MyDrive/NLP_project/


File name required:

inspirational_quotes.txt

**Step 3: Add the Python Script**

Paste the full Python code into Colab.

Make sure the paths are:

FILE_PATH = '/content/drive/MyDrive/NLP_project/inspirational_quotes.txt'
CSV_OUTPUT = '/content/drive/MyDrive/NLP_project/results_inspirational_quotes.csv'
DB_OUTPUT = '/content/drive/MyDrive/NLP_project/results_inspirational_quotes.db'
RULE_PLAN_CSV = '/content/drive/MyDrive/NLP_project/rule_plan.csv'

**Step 4: Connect Google Drive**

Run:

from google.colab import drive
drive.mount('/content/drive')

**Step 5: Run the Main Function**

Execute:

main()


This triggers:

Text cleaning

Chunking

Parallel processing

Word count

Rule detections

CSV + DB saving

Chart generation

**Step 6: Output Files Generated Automatically**

Stored in:

/content/drive/MyDrive/NLP_project/

Files created:

results_inspiritional_quotes.csv

results_inspirational_quotes.db

rule_plan.csv

Bar chart

Pie chart

**Step 7: View or Download Outputs**

CSV → open in Excel/Sheets

DB → open in DB Browser for SQLite

Charts → appear directly in Colab

Rule matches → printed in console

**5. Rule-Based Detection System**
Rule Name	Purpose
Positive Word Detector	Detect motivational keywords
Hope + Struggle Detector	Identify quotes combining hope with struggle
Long Quote Detector	Finds quotes containing more than 20 words
Action Word Detector	Detects verbs like start, act, begin, rise
Emotion Word Detector	Detects love, care, kindness, joy
Wisdom Word Detector	Detects learn, teach, understand
Negation Detector	Detects words like not, never, don’t
Question Detector	Detects presence of “?”

**6. Expected Output**
CSV of Positive Word Counts

Example:

word,frequency
hope,120
dream,95
success,80

Bar Chart

Displays frequency of each positive word.
![WhatsApp Image 2025-12-04 at 21 18 17_34deb9aa](https://github.com/user-attachments/assets/31653cd7-7ace-46f0-8f38-d1ac57bd970d)


Pie Chart

Shows percentage contribution of each word.
![WhatsApp Image 2025-12-04 at 21 16 59_a2338030](https://github.com/user-attachments/assets/80101289-2252-4a81-80fd-b2c013666bc9)


**7. Conclusion**

This project provides strong practical experience in:

Text analysis

NLP preprocessing

Word frequency modeling

Rule-based NLP

Data visualization

CSV and SQL storage

It reveals which motivational themes dominate inspirational literature and builds essential skills for NLP, data
