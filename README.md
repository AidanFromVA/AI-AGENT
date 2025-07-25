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
│   ├── recommender.py            # Resume-based job recommendation engine
│   └── resume_parser.py          # PDF/Text resume parsing and keyword extraction
│
├── ai/
│   ├── prompt_templates/    
│   │   ├── cover_letter.txt      # Prompt template for GPT-generated cover letters
│   │   └── interview_prompt.txt  # Prompt template for interview Q&A
│   ├── generator.py              # GPT-based cover letter and question generator
│   └── langchain_agent.py        # LangChain agent for orchestrating multi-step flows
│
├── frontend/
│   ├── streamlit_app.py          # Streamlit web UI for user interaction
│   └── pages/                    # Optional extra pages: dashboard, history, etc.
│
└── README.md                     # Project documentation and instructions
