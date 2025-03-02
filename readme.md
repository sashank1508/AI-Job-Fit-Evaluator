# AI-Powered Job Fit Evaluator

## 🚀 Overview

This project is an **AI-driven job fit evaluator** that automates the process of assessing a candidate's suitability for a job role. It does so by:

✔ Scraping **LinkedIn profile data** using **Selenium**  
✔ Extracting **resume information** from a **PDF** file  
✔ Comparing both with a **Job Description**  
✔ Using **OpenAI's GPT model** to analyze strengths, weaknesses, and provide a suitability rating  

This tool is designed to help recruiters, hiring managers, or candidates themselves get a **data-driven assessment** of a profile’s alignment with a given role.

---

## 📜 Features

✔ **Automated LinkedIn Scraping** – Extracts profile details including name, headline, location, connections, and about section  
✔ **LinkedIn Profile to PDF Conversion** – Downloads and stores the candidate’s profile as a PDF  
✔ **Resume Parsing** – Reads and extracts text from a candidate’s resume (PDF)  
✔ **AI-based Job Fit Analysis** – Uses **GPT** to compare the LinkedIn profile & resume against a Job Description  
✔ **Strengths & Weaknesses Assessment** – AI highlights key qualifications and potential gaps  
✔ **Suitability Score** – Rates the candidate on a scale of **1 to 10** for the given job role  
✔ **Automated Execution** – Runs the entire process asynchronously for efficiency  

---

## 🛠️ Tech Stack

| Technology      | Purpose                                                        |
|---------------|----------------------------------------------------------------|
| **Python** | Core programming language for automation & AI evaluation |
| **Selenium** | Web scraping automation to extract LinkedIn profile data |
| **PyMuPDF** | PDF parsing to extract text from LinkedIn profiles & resumes |
| **OpenAI GPT API** | AI-driven job fit analysis and candidate evaluation |
| **AsyncIO** | Handles asynchronous execution for efficiency |
| **dotenv** | Manages API keys and credentials securely |
| **Logging** | Tracks script execution and error handling |

---

## 📦 System Workflow

1️⃣ **Selenium logs into LinkedIn** using stored credentials  
2️⃣ **Navigates to the candidate’s profile and extracts key details**  
3️⃣ **Downloads the LinkedIn profile as a PDF** for further processing  
4️⃣ **Extracts text from both the LinkedIn profile PDF & Resume PDF**  
5️⃣ **AI model (GPT) compares LinkedIn, Resume, and Job Description**  
6️⃣ **Generates an evaluation report with strengths, weaknesses & rating**  
7️⃣ **Final assessment is displayed to the user**  

---

## 🏗️ Setup & Installation

### **🔹 Prerequisites**

- Python 3.8+
- Google Chrome & ChromeDriver installed
- OpenAI API key
- LinkedIn credentials (stored in a `.env` file)

### **🔹 Clone the Repository**

```sh
git clone https://github.com/sashank1508/ai-job-fit-evaluator
cd ai-job-fit-evaluator
```

### **🔹 Create a Virtual Environment**

```sh
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### **🔹 Install Dependencies**

```sh
pip install -r requirements.txt
```

### **🔹 Configure Environment Variables**

Create a `.env` file in the project directory and add:

```ini
LINKEDIN_EMAIL=your-email@example.com
LINKEDIN_PASSWORD=your-password
OPENAI_API_KEY=your-openai-api-key
```

### **🔹 Run the main.ipynb Notebook**

---

## ⚡ How It Works

1. **Extracts Data from LinkedIn Profile**
   - Logs in with stored credentials
   - Scrapes profile data
   - Saves profile details as a PDF

2. **Extracts Resume Data**
   - Reads resume text from a PDF

3. **Compares with Job Description**
   - Uses OpenAI GPT to evaluate strengths & weaknesses
   - Rates the candidate’s suitability for the role

4. **Generates Evaluation Report**
   - Outputs structured analysis & score (1-10)

---

## 📊 Example Output

```plaintext
Candidate: Sashank Yendrapati
Headline: Backend Engineer at Quicksell
Location: Mumbai, India
Connections: 500+
Followers: 1000+

✅ Strengths:
- Extensive experience with LLMs & AI models
- Strong knowledge of NLP and transformers
- Proficiency in PyTorch & TensorFlow
- Hands-on experience with Retrieval-Augmented Generation (RAG)
- Experience with cloud platforms

❗Areas for Improvement:
- Limited experience with MLOps
- Could gain more experience in model deployment at scale
- Not highlighted any formal leadership or mentoring experience

📌 **Final Recommendation:** Strong fit for the AI Engineer role with minor improvements.
🎯 **Suitability Score:** 8.5/10
```

---

## 🔧 Future Enhancements

🔹 **Improve LinkedIn Scraping Method** – Use alternative methods to avoid detection  
🔹 **Add Support for More Resume Formats** – DOCX, TXT parsing  
🔹 **Deploy as a Web App** – Convert into a web-based tool for recruiters  
🔹 **Enhance AI Model Prompts** – Fine-tune LLM evaluations for better accuracy  
🔹 **Optimize PDF Processing** – Extract specific sections for better comparisons  

---

## 📝 Author

👨‍💻 **Sashank Yendrapati**  
📧 Email: <sashank1.y@gmail.com>  
🔗 LinkedIn: [Sashank's Profile](https://www.linkedin.com/in/sashank-yendrapati-358498a5/)  
📁 GitHub: [sashank1508](https://github.com/sashank1508)

---
