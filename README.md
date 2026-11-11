# 🚀 Candidate Resume Screening System

A Python-based **Candidate Resume Screening System** developed using Object-Oriented Programming (OOP) principles. This application automates the initial candidate evaluation process by matching technical skills, checking experience eligibility, validating educational qualifications, and generating screening reports.

## 📌 Project Overview

The Candidate Resume Screening System is designed to simplify the initial recruitment and candidate shortlisting process.

It allows recruiters to create job openings, register Fresher and Experienced candidates, evaluate their profiles against job requirements, and identify suitable candidates based on predefined eligibility criteria.

The system also provides a keyword-based candidate search functionality to find candidates based on their technical skills and job roles.

## 🎯 Problem Statement

Manual resume screening can be time-consuming, especially when recruiters need to evaluate multiple candidates against different job requirements.

This project addresses the problem by implementing a structured screening mechanism that:

- Evaluates candidate skills against required job skills.
- Calculates skill-match percentages.
- Checks minimum years of experience.
- Validates educational qualifications.
- Applies CGPA requirements for freshers.
- Automatically shortlists or rejects candidates.
- Provides keyword-based candidate searching.
- Generates detailed screening reports.

## ✨ Key Features

- **Job Management:** Create job openings with required skills, qualifications, experience, CGPA, and minimum skill-match percentage.
- **Candidate Registration:** Register both Fresher and Experienced candidates.
- **Skill Matching:** Identify matched and missing skills.
- **Percentage Calculation:** Calculate candidate skill-match percentages.
- **Experience Validation:** Evaluate professional experience and internship experience.
- **Qualification Validation:** Verify whether candidate qualifications meet job requirements.
- **Automated Screening:** Classify candidates as Shortlisted or Rejected.
- **Keyword Search:** Search candidates using skills, job roles, and categories.
- **Input Validation:** Validate candidate details and job requirements.
- **Exception Handling:** Handle invalid inputs and application errors.
- **Screening Reports:** Generate detailed candidate evaluation reports.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| ABC | Abstract classes and methods |
| Dataclasses | Structured screening result objects |
| Random | Keyword number generation |
| RE (Regular Expressions) | Email validation and text normalization |
| Textwrap | Formatting role information |
| Typing | Type hints and structured annotations |

**External Dependencies:** None. The project uses Python standard-library modules.

## 🧠 Object-Oriented Programming Concepts

This project demonstrates all four pillars of Object-Oriented Programming.

### 1. Encapsulation
- Uses private attributes to protect candidate and job information.
- Implements getter and setter methods through Python properties.
- Performs validation before updating important attributes.

### 2. Abstraction
- Uses the `ABC` module to define abstract classes.
- Implements abstract methods for candidate screening, searching, displaying details, and job roles.
- Ensures child classes provide their required implementations.

### 3. Inheritance
- `FresherCandidate` and `ExperiencedCandidate` inherit from the `Candidate` class.
- Specialized job roles inherit from common role categories.
- Reuses common functionality through parent classes.

### 4. Polymorphism
- Different candidate types implement their own experience eligibility checks.
- Different job roles implement their own `work()` methods.
- Common screening operations work with different candidate objects.

## ⚙️ How It Works

The application follows a three-step workflow.

### Step 1: Job Opening

Enter the following job details:

- Job Title
- Company Name
- Required Skills
- Accepted Qualifications
- Minimum Years of Experience
- Minimum CGPA for Freshers
- Minimum Skill Match Percentage

### Step 2: Candidate Registration

Register candidates by selecting their candidate type.

**Fresher Candidate:**
- Candidate Name
- Email Address
- Qualification
- Technical Skills
- Job Role
- CGPA
- Internship Duration

**Experienced Candidate:**
- Candidate Name
- Email Address
- Qualification
- Technical Skills
- Job Role
- Years of Experience
- Current Company

### Step 3: Candidate Screening

The system evaluates each candidate based on:

1. Skill matching.
2. Skill-match percentage calculation.
3. Experience eligibility.
4. Qualification validation.
5. Minimum eligibility requirements.

Candidates meeting all configured requirements are marked as **Shortlisted**. Candidates failing one or more requirements are marked as **Rejected**, with reasons displayed in the report.

### Skill Match Formula

```text
Skill Match Percentage =
(Matched Skills / Total Required Skills) × 100
```

For example:

```text
Required Skills: Python, SQL, Django, React

Candidate Skills: Python, SQL, Django

Matched Skills: 3
Missing Skills: 1

Skill Match = (3 / 4) × 100

Skill Match Percentage = 75%
```

## 🔍 Candidate Search Functionality

The application includes a keyword-based candidate search system.

Users can search candidates using:

- Technical skills
- Job role titles
- Job role categories
- Candidate names

The search system calculates a relevance score, sorts matching candidates, and displays the results.

It also supports predefined keyword synonym groups for selected AI/ML and Generative AI terms.

## 📂 Project Structure

```text
CANDIDATE-RESUME-SCREENING-SYSTEM/
│
├── CANDIDATE RESUME SCREENING SYSTEM.ipynb
│
└── README.md
```

The current implementation is provided as a Jupyter Notebook.

## 💻 Installation & Execution

### Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab

### Step 1: Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

### Step 2: Navigate to the Project Directory

```bash
cd CANDIDATE-RESUME-SCREENING-SYSTEM
```

### Step 3: Install Jupyter Notebook

```bash
pip install notebook
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Project

Open the following notebook:

```text
CANDIDATE RESUME SCREENING SYSTEM.ipynb
```

Run the cells and follow the interactive instructions.

## 📊 Sample Data

The application includes built-in sample data.

It provides:

- 10 sample candidates.
- 2 sample job openings.
- Fresher and Experienced candidate profiles.
- AI/ML and Generative AI job roles.

You can choose to use the sample data or enter your own job and candidate details.

## 📋 Screening Results

The screening report displays:

| Evaluation | Description |
|---|---|
| Skill Match | Matched skill percentage |
| Experience | Eligible / Not eligible |
| Qualification | Accepted / Not accepted |
| Status | Shortlisted / Rejected |

The report also displays matched skills, missing skills, and rejection reasons for each candidate.

## 🌍 Real-World Applications

This project demonstrates functionality relevant to:

- HR Recruitment Management Systems.
- Applicant Tracking Systems (ATS).
- Technical Recruitment Platforms.
- Fresher Recruitment and Evaluation.
- Experienced Candidate Shortlisting.
- Skill-Based Candidate Search.
- Job Portal Candidate Management.

## 📚 My Learnings

Through this project, I gained practical experience in:

- Implementing the four pillars of OOP.
- Designing abstract classes and interfaces.
- Understanding inheritance and method overriding.
- Implementing encapsulation with private attributes and properties.
- Applying polymorphism in real-world scenarios.
- Building custom exception classes.
- Performing data validation.
- Working with Python standard-library modules.
- Developing reusable and maintainable application logic.
- Designing a complete interactive Python mini project.

## 🚀 Future Enhancements

Potential improvements for future versions:

- PDF and DOCX resume upload and text extraction.
- Database integration using SQLite or MySQL.
- Graphical User Interface (GUI).
- Web-based recruitment dashboard.
- Advanced skill matching using NLP.
- Candidate profile management.
- Export screening reports to PDF or Excel.
- AI-assisted candidate recommendations.

## 👨‍💻 Author

**Developed as a Python OOP Mini Project**

If you find this project useful, consider giving the repository a ⭐ on GitHub.

## 📌 Project Note

This is an initial rule-based screening application. It evaluates structured candidate information entered by the user; it does not currently parse uploaded resume documents or use machine learning to make recruitment decisions.

---

**Technologies:** Python | OOP | Encapsulation | Abstraction | Inheritance | Polymorphism

#Python #PythonProjects #OOP #ResumeScreening #SoftwareDevelopment
