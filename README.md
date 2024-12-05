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

## How It Works

### 1. **Data Input**
   - Job description is entered as plain text.
   - Resume is uploaded and parsed to extract text.

### 2. **Data Preprocessing**
   - **Tokenization**: Breaks down text into individual words or tokens.
   - **Stopword Removal**: Common words (e.g., "and", "the") are removed to focus on meaningful keywords.
   - **Stemming/Lemmatization**: Reduces words to their root forms (e.g., "running" → "run").
   - **Normalization**: Converts text to lowercase to ensure case-insensitive matching.

### 3. **Prompt Engineering**
   - A carefully crafted prompt is sent to the Gemini model to ensure effective semantic analysis.
   - Example prompt:
     ```
     Analyze the job description and the resume. Identify and list:
     1. Keywords or phrases common between the two.
     2. Keywords from the job description missing in the resume.
     Provide the results as two separate lists.
     ```

### 4. **AI Model Analysis**
   - The **Gemini model** processes the job description and resume text to:
     - Extract keywords using semantic understanding.
     - Match contextually relevant words (e.g., recognizing synonyms like "develop" and "build").
     - Highlight gaps to provide actionable feedback.

### 5. **Result Display**
   - Outputs two lists:
     - **Existing Keywords**: A list of matched words/phrases.
     - **Missing Keywords**: A list of job description words/phrases absent in the resume.
   - Results are displayed in a user-friendly format, such as tables or charts.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/whoisusmanali/Resume-Application-Tracking-System-ATS-Using-Google-Gemini.git
   cd Resume-Application-Tracking-System-ATS-Using-Google-Gemini
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   streamlit run app.py
   ```

---

## Usage

1. **Launch the application**:
   - Run the `app.py` script and access the app in your web browser.

2. **Input Data**:
   - Paste the job description in the designated text area.
   - Upload the resume file.

3. **View Results**:
   - Review the detailed breakdown of missing and existing keywords.
   - Use the insights to improve resume alignment with the job description.

---

## Future Enhancements

1. **Multi-format Resume Parsing**:
   - Support for additional file types like `.docx`.

2. **Advanced Semantic Analysis**:
   - Include weightage for skill importance.

3. **Visualization**:
   - Add bar charts or word clouds for visual representation of the analysis.

4. **Customization**:
   - Allow users to specify the importance of certain keywords.


## Acknowledgments

- **Google Gemini Model**: For powering the semantic analysis.
- **Streamlit**: For making the interface simple and user-friendly.
- **Python Libraries**: For facilitating data processing and analysis.

--- 

### Contact
For questions, feedback, or collaboration, please reach out at [whoisusmanali@gmail.com](whoisusmanali@gmail.com).