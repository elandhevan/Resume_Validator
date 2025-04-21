# 📝 Resume Validator

A smart **AI-powered Applicant Tracking System (ATS)** that analyzes resumes against job descriptions using **Google Gemini**. This tool provides two powerful modes:
1. **HR Evaluation** – Detailed professional feedback.
2. **ATS Match %** – Keyword-based match scoring with missing keyword highlights.

---

## 🚀 Features

- 📄 Upload resume in PDF format
- 📃 Paste job description
- 🔎 Analyze with generative AI (Google Gemini)
- 📈 Get match percentage + missing keyword insights
- 🧠 Dual-mode AI prompts (HR + ATS)
- 🎨 Stylish custom Streamlit UI with animations
- 🖥️ Fully local and open-source

---

## 🧰 Tech Stack

- **Frontend & UI**: Streamlit (with custom CSS)
- **Backend & AI**: Google Gemini via `google-generativeai`
- **PDF Handling**: pdf2image + Poppler + Pillow
- **Environment Management**: python-dotenv

---

## ⚙️ Installation & Setup

### 1. Clone the repo

```bash
git clone https://github.com/your-username/resume-validator.git
cd resume-validator
```

### 2. Install Python packages

```bash
pip install -r requirements.txt
```

### 3. Install Poppler (for `pdf2image`)

#### On Windows:
- Download: [https://github.com/oschwartz10612/poppler-windows/releases](https://github.com/oschwartz10612/poppler-windows/releases)
- Extract to: `D:\resume_validator\poppler`
- Update this line in `app.py` with your actual path:

```python
poppler_path=r"D:\resume_validator\poppler\bin"
```

---

### 4. Set up Google Gemini API

- Go to: [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)
- Create an API Key
- Create a `.env` file in the project root:

```env
GOOGLE_API_KEY=your_actual_api_key
```

---

### 5. Run the app

```bash
streamlit run app.py
```

Then open [http://localhost:8501](http://localhost:8501) in your browser.

---

## 📂 File Structure

```bash
.
├── app.py                # Main Streamlit app
├── requirements.txt      # Python dependencies
├── packages.txt          # Linux system dependencies
├── .env                  # Your Google API Key (not committed)
├── README.md             # Project documentation
```

---

## ✅ Sample Job Descriptions

To test your app, try roles like:
- Full Stack Developer (React + Node.js)
- Data Scientist
- DevOps Engineer

You can copy job descriptions from LinkedIn or Indeed.

---

## 🙌 Credits

Built by **Team Twix**  
Powered by Google Gemini + Streamlit

---

## 📄 License

This project is open-source and available under the MIT License.
