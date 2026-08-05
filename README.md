Add files via upload
AI-Powered Resume Screening System
An AI-powered recruitment tool that analyzes candidate resumes, compares them with recruiter-defined job requirements, calculates a job-matching score, and provides clear shortlisting or rejection reasons.

The project uses Python and Groq LLM to automate the initial resume-screening process.

Features
Extracts information from PDF and DOCX resumes
Identifies candidate skills, education, experience, and projects
Accepts recruiter-defined job requirements
Compares candidate skills with the required skills
Calculates a matching score from 0% to 100%
Recommends candidates scoring 80% or higher
Sends candidates scoring 70% to 79% for manual review
Rejects candidates scoring below 70%
Explains missing skills and reasons for rejection
Produces structured results using Pydantic and JSON
Candidate Selection Criteria
Matching Score	Result
80%–100%	Shortlisted for Interview
70%–79%	Manual Recruiter Review
Below 70%	Rejected
Matching Criteria
Category	Weight
Required Skills	40%
Relevant Experience	25%
Projects	15%
Education	10%
Tools and Certifications	10%
Technologies Used
Python
Groq API
Large Language Models
Pydantic
PDFPlumber
python-docx
JSON
Regular Expressions
Prompt Engineering
Natural Language Processing
Project Structure
text resume-screening-system/ ├── app.py ├── resume_parser.py ├── matcher.py ├── models.py ├── requirements.txt ├── .env.example ├── .gitignore ├── resumes/ └── README.md
main
