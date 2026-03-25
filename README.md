# ASLAB — Assessment Lab

ASLAB (Assessment Lab) is a lightweight web-based tool designed to automate post-exam item analysis across multiple subjects and students

Instead of manually encoding and analyzing test results, ASLAB processes structured data and instantly generates per-subject item analysis, difficulty indices, discrimination indices, and actionable insights.

After exams, teachers often:

* Handle dozens of students (50+)
* Work across multiple subjects
* Manually encode responses into spreadsheets
* Perform repetitive calculations for item analysis
* Spend significant time organizing and interpreting results

This process is:

* Time-consuming
* Error-prone
* Difficult to scale

ASLAB simplifies this workflow by allowing teachers to:

* Input multi-subject student responses
* Automatically group and process data
* Generate item analysis instantly
* Identify problematic, effective, and weak questions

All in a single analysis run

---

Features

Multi-Subject Analysis

* Automatically detects and separates subjects
* Runs item analysis per subject without manual grouping

Core Metrics

* Difficulty Index (how easy or hard a question is)
* Discrimination Index (how well a question differentiates students)

 Smart Actions

Each question is automatically classified:

* KEEP — effective item
* REVISE — needs improvement
* REMOVE — problematic or misleading

Insights Generation

* Flags unusually easy or difficult questions
* Detects negative discrimination
* Highlights potential issues in test design

---

Input Format

Data should be provided in CSV-style format:

```
StudentID,Subject,Q1,Q2,Q3,Q4,Q5
Student1,Math,A,B,C,D,A
Student1,Science,B,B,C,D,A
Student2,Math,A,B,D,D,A
Student2,Science,B,C,C,D,A
```

---

How to Run

1. Download or clone the repository
2. Open the `index.html` (or your HTML file) in any browser
3. Paste your dataset into the input field
4. Click "Analyze All Subjects"

No installation required.

---

How It Works

For each subject:

* Determines the answer key (most frequent response per question)
* Calculates:

  * Difficulty Index
  * Discrimination Index (Top 27% vs Bottom 27%)
* Generates:

  * Action labels (Keep / Revise / Remove)
  * Insights based on performance patterns

---

Project Goal

ASLAB is built to:

> Reduce post-exam workload and eliminate repetitive data processing, allowing teachers to focus on improving assessments instead of managing data.

---
 Current Status

* ✅ Functional prototype
* ✅ Multi-subject support
* ✅ Basic UI and analysis engine

Planned improvements:

* File upload (CSV import)
* Export reports (PDF / Excel)
* Enhanced insights system
* Improved UI/UX

---

Author

Developed by a student focused on building practical tools for real-world academic workflows.

---

License

This project is open for educational and research purposes.
