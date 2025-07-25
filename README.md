# 🧠 AI-AGENT: Your Personal Job Search Assistant
**AGENT WILL SAVE YOU.**

AI-AGENT is an intelligent job-search assistant that helps users find relevant job opportunities, analyze their resumes, recommend positions, and generate personalized cover letters using AI.

---

## 🚀 Key Features

- 📄 **Resume Parsing**: Extract skills and experience from uploaded PDF resumes  
- 🔍 **Job Recommendation**: Match jobs based on resume content using AI similarity scoring  
- ✍️ **Cover Letter Generation**: Create tailored cover letters with OpenAI GPT  
- 🧠 **Agent Flow**: LangChain-based pipeline for chaining resume analysis → recommendation → cover letter generation  
- 💻 **Streamlit UI**: User-friendly interface to upload, view recommendations, and download generated letters

---

## 📁 Project Structure

job_agent/
│
├── backend/
│   ├── app.py                    # FastAPI or Flask API server
│   ├── scraper/
│   │   └── linkedin.py           # Job listing scraper (future extension)
│   ├── recommender.py            # AI-powered job recommender based on resume
│   └── resume_parser.py          # Extract info from PDF/Text resumes
│
├── ai/
│   ├── prompt_templates/
│   │   ├── cover_letter.txt      # Template for GPT cover letter prompt
│   │   └── interview_prompt.txt  # Template for GPT interview Q&A
│   ├── generator.py              # GPT-based text generation logic
│   └── langchain_agent.py        # LangChain-based pipeline handler
│
├── frontend/
│   ├── streamlit_app.py          # Streamlit UI entry point
│   └── pages/                    # Optional: dashboard, saved results, etc.
│
└── README.md                     # Project documentation

