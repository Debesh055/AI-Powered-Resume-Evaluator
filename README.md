# 🤖 AI-Powered Resume Screening System

> An intelligent AI-based recruitment tool that automates resume screening using the **Groq API**. The system extracts information from PDF and DOCX resumes, compares candidate profiles with recruiter-defined job requirements, calculates an ATS-style matching score, and provides transparent hiring recommendations.

---

## 📌 Features

- 📄 Extracts data from **PDF** and **DOCX** resumes
- 🧠 AI-powered resume analysis using **Groq LLM**
- 🎯 Matches resumes against recruiter-defined job requirements
- 📊 Calculates a **0–100% job matching score**
- 💼 Extracts:
  - Skills
  - Education
  - Experience
  - Projects
  - Certifications
- ✅ Shortlists qualified candidates
- ⚠️ Flags borderline candidates for manual review
- ❌ Rejects unsuitable candidates with clear reasons
- 📋 Identifies missing skills and qualification gaps
- 📦 Returns structured JSON output using **Pydantic**

---

## 🎯 Candidate Selection Criteria

| Matching Score | Decision |
|---------------|----------|
| **80% – 100%** | ✅ Shortlisted for Interview |
| **70% – 79%** | ⚠️ Manual Recruiter Review |
| **Below 70%** | ❌ Rejected |

---

## 📊 Matching Criteria

| Category | Weight |
|----------|--------|
| Required Skills | **40%** |
| Relevant Experience | **25%** |
| Projects | **15%** |
| Education | **10%** |
| Tools & Certifications | **10%** |

---

## 🛠️ Tech Stack

- 🐍 Python
- ⚡ Groq API (LLM)
- 📄 PDFPlumber
- 📃 python-docx
- 📦 Pydantic
- 🧩 JSON
- ✍️ Prompt Engineering
- 🤖 Natural Language Processing (NLP)

---

## 📁 Project Structure

```text
resume-screening-system/
│
├── matcher.py
├── resume_parser.py
├── models.py
├── requirements.txt
├── .env.example
├── .gitignore
├── resumes/
└── README.md
```

---

## 🚀 How It Works

1. Upload a candidate's resume (PDF/DOCX)
2. Enter the job description or required skills
3. AI extracts candidate information
4. Resume is compared with job requirements
5. Matching score is calculated
6. System generates:
   - ATS Match Score
   - Hiring Decision
   - Missing Skills
   - Improvement Suggestions
   - Structured JSON Output

---

## 📈 Sample Output

```json
{
  "candidate_name": "John Doe",
  "match_score": 86,
  "decision": "Shortlisted",
  "missing_skills": [
    "Docker",
    "AWS"
  ],
  "reason": "Strong technical skills and relevant project experience."
}
```

---

## 🔮 Future Improvements

- Resume ranking dashboard
- Multiple resume screening
- Recruiter login system
- Candidate database
- Streamlit/Web interface
- Email notifications
- Export reports to PDF
- Advanced ATS keyword analysis

---

## 👨‍💻 Author

**Debesh Mandal**

📧 Feel free to connect and contribute!

---

### ⭐ If you found this project useful, don't forget to Star the repository!
