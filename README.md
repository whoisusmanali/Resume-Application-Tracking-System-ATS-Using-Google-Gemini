# Resume Application Tracking System ATS Using Google Gemini

This project is a **Streamlit-based web application** designed to help job seekers analyze the alignment between their resumes and job descriptions. By leveraging **Google's Gemini model**, the application compares the content of a resume with a job description, identifies overlapping keywords, and highlights missing ones to provide actionable insights for improving resume alignment.

---

## Features

1. **Interactive Interface**: 
   - **Input Area 1**: Paste the job description.
   - **Input Area 2**: Upload the resume (in plain text or supported formats like `.txt` or `.pdf`).
   
2. **Keyword Matching**:
   - Matches keywords from the job description with those in the resume.
   - Displays insights into:
     - **Existing Keywords**: Words that match between the resume and the job description.
     - **Missing Keywords**: Words present in the job description but missing in the resume.
   
3. **Powered by Gemini LLM**:
   - Utilizes Google's Gemini model for text processing and semantic matching.
   - Provides accurate analysis by understanding context, synonyms, and related phrases.

---

## Technology Stack

- **Frontend**: Streamlit (for building an intuitive user interface).
- **Backend**: Gemini LLM (Large Language Model) for keyword extraction and semantic matching.
- **Languages**: Python.
- **Libraries**: 
  - `streamlit` for UI.
  - `pandas` for data handling.
  - `PyPDF2` or `pdfplumber` for parsing PDF resumes.
  - `nltk` or `spaCy` for text preprocessing.

---
