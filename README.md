# -intelligent_resume_analyzer_hidevs
# Intelligent Resume Analyzer

A Python-based application that automates resume screening by:

- Extracting candidate information
- Matching skills with job requirements
- Calculating match scores
- Generating hiring recommendations
- Saving reports in JSON format

## Technologies Used
- Python
- Regex
- JSON

## Output
The system generates:
- Candidate analysis
- Match score
- Hiring recommendation
- JSON report

# Features

- Extracts candidate name from resume
- Extracts email address using Regular Expressions
- Detects technical skills from resume text
- Extracts years of experience
- Matches candidate skills with required job skills
- Calculates match score (0–100)
- Generates hiring recommendations
- Saves reports in JSON format
- Handles invalid or missing input gracefully

# Technologies Used

| Technology | Purpose |
| Python | Core programming language |
| Regex (`re`) | Text extraction and parsing |
| JSON | Saving analysis reports |
| Datetime | Timestamp generation |

---

# Project Workflow

```text
Resume Input
     ↓
Text Parsing
     ↓
Information Extraction
     ↓
Skill Matching
     ↓
Score Calculation
     ↓
Recommendation Generation
     ↓
JSON Report Creation
```

---

# Project Structure

```text
intelligent_resume_analyzer_hidevs/
│
├── main.py
├── report.json
├── README.md
```

---

# Resume Information Extracted

The system extracts the following details:

- Candidate Name
- Email Address
- Skills
- Years of Experience

---

# Match Score Calculation

The final score is calculated based on:

- Skill Match Percentage
- Experience Match

## Formula

```python
Final Score =
(Skill Score × 70%) +
(Experience Score × 30%)
```

---

# Hiring Recommendation Logic

| Score Range | Recommendation |
|---|---|
| 80 – 100 | Strong Hire |
| 60 – 79 | Consider |
| Below 60 | Reject |

---

# Sample Resume Input

```text
Name: John Doe

Email: john.doe@gmail.com

Skills:
Python, SQL, Machine Learning,
Pandas, Data Analysis

Experience:
3 years as Data Analyst
```

---

# Sample Output

```text
===== RESUME ANALYSIS =====

candidate_name: John Doe
email: john.doe@gmail.com
skills_found:
['Python', 'SQL', 'Machine Learning',
'Pandas', 'Data Analysis']

matched_skills:
['Python', 'SQL', 'Machine Learning',
'Pandas', 'Data Analysis']

experience: 3
match_score: 100.0
recommendation: Strong Hire
```

---

# JSON Report Example

```json
{
    "candidate_name": "John Doe",
    "email": "john.doe@gmail.com",
    "skills_found": [
        "Python",
        "SQL",
        "Machine Learning"
    ],
    "matched_skills": [
        "Python",
        "SQL"
    ],
    "experience": 3,
    "match_score": 82.5,
    "recommendation": "Strong Hire"
}
```

---

# How To Run The Project

## Step 1: Clone Repository

```bash
git clone https://github.com/your-username/intelligent_resume_analyzer_hidevs.git
```

---

## Step 2: Open Project Folder

```bash
cd intelligent_resume_analyzer_hidevs
```



## Step 3: Run Python File

```bash
python main.py
```


# Error Handling

The system handles:

- Missing email addresses
- Missing names
- Invalid resume formats
- Empty input data
- Missing experience values


# Advantages of the System

- Reduces manual HR effort
- Faster candidate screening
- Consistent evaluation process
- Structured analysis reports
- Easy to extend and customize

# Future Improvements

Possible future enhancements include:

- PDF Resume Support
- Multiple Resume Analysis
- Streamlit Web Interface
- Machine Learning-based Skill Matching
- NLP-based Resume Parsing
- Database Integration
- ATS Integration

# Industry Applications

This project can be used in:

- Recruitment Platforms
- HR Technology Systems
- Applicant Tracking Systems (ATS)
- Job Portals
- Talent Acquisition Teams

# Learning Outcomes

Through this project, the following skills were developed:

- Python Programming
- Text Processing
- Regular Expressions
- JSON File Handling
- Matching Algorithms
- Error Handling
- Report Generation


# Author

Developed as part of the HiDevs Intelligent Resume Analyzer Project.
