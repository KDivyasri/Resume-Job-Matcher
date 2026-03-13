
# 📄 Resume & Job Matcher

## 🚀 Overview

This application allows you to upload a **Resume** and a **Job Description**, then uses a **local Large Language Model (LLM)** via **Ollama** to analyze how well they match.

The app evaluates the resume against the job requirements and provides actionable insights.

### The analysis includes:

- ✅ **Fit Score (0–100%)** indicating resume–job alignment  
- 💪 **Key strengths** showing areas where the resume matches the job well  
- 📝 **Personalized improvement suggestions** tailored to the job description  

Additionally, the app generates a **downloadable Match Report** so users can keep a record of the analysis.

---

# 🛠️ Tech Stack

- **Python**
- **Streamlit** – interactive web interface
- **Ollama + LLM (e.g., llama3)** – local AI analysis
- **PyMuPDF** – PDF text extraction
- **Requests** – communication with Ollama API

---

# ⚡ Setup Instructions

## 1️⃣ Install dependencies

Install all required Python libraries:

```
pip install -r requirements.txt
```

---

## 2️⃣ Install Ollama

Download and install Ollama:

https://ollama.ai

Ollama allows you to run **LLMs locally on your machine**.

---

## 3️⃣ Run the Ollama model

Pull and start the model:

```
ollama run llama3
```

If Ollama is already running in the background, you may see:

```
address already in use
```

This is normal and means the Ollama server is already active.

---

## 4️⃣ Start the application

Run the Streamlit app:

```
streamlit run app.py
```

---

## 5️⃣ Open the app

After running the command above, open your browser and navigate to:

```
http://localhost:8501
```

---

# 📊 How the App Works

1. Upload your **Resume (PDF)**  
2. Upload the **Job Description (PDF)**  
3. Click **Match Resume with Job Description**  
4. The LLM analyzes the documents and generates:

- Fit Score
- Resume strengths
- Missing skill areas
- Improvement recommendations

---

# 📥 Download Match Report

After the analysis is generated, you can download the full report.

The app provides a **Download Match Report** button that saves the analysis as a **Markdown (`.md`) file**.

This report contains:

- Fit Score
- Highlight Resume strengths
- Improvement suggestions

This allows users to **save, review, or share the results easily**.

---

# 💡 Example Use Cases

- Job seekers optimizing resumes for specific roles
- Students preparing resumes for internships
- Professionals tailoring resumes for ATS systems
- Quick resume-job alignment checks before applying

---

