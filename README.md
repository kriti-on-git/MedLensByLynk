# MedLensByLynk

## 🩺 **MedLens — AI-Powered Medical Report Analyzer**

### 🔍 **Project Description**

MedLens is an AI-driven health analysis tool that decodes your medical reports in seconds.
Upload your lab report (PDF or image), and MedLens extracts key health metrics like sugar, cholesterol, hemoglobin, etc., visualizes them, and explains their medical meaning — all in plain English.

The goal is to make diagnostic insights understandable to *anyone*, not just doctors. 
Fun Addition: Doctor Funshine (Fun personas reading your reports)

---

## 🧩 **Problem Statement**

Most people receive medical test reports full of complex terms, abbreviations, and numeric ranges they can’t interpret.
This creates confusion, anxiety, and dependence on external help — even for basic understanding.

We aim to bridge this communication gap between **medical data** and **human understanding**.

---

## 💡 **Proposed Solution**

MedLens leverages **OCR + AI-based interpretation** to:

1. Read medical reports intelligently (PDF or image).
2. Extract vital health metrics.
3. Generate easy-to-understand health summaries.
4. Visualize each parameter using intuitive graphs — comparing actual vs. normal values.

Built for accessibility, MedLens simplifies medical literacy for everyone.

---

## ⚙️ **Technology Stack**

| Layer                   | Tools / Frameworks Used                                   |
| ----------------------- | --------------------------------------------------------- |
| **Frontend/UI**         | Streamlit (custom dark theme, responsive dashboard)       |
| **AI/ML Backend**       | Google Gemini API (for report interpretation & summaries) |
| **OCR/Extraction**      | Python `pytesseract`, `Pillow`, and `pdf2image`           |                                      |
| **Deployment**          | Streamlit Community Cloud (public URL)                    |
| **Version Control**     | Git + GitHub                                              |

---

## 🏗️ **Architecture / Design**

```
                ┌────────────────────────────┐
                │   User uploads report       │
                └─────────────┬───────────────┘
                              │
                              ▼
                  [OCR Extraction Layer]
             (pytesseract + pdf2image + Pillow)
                              │
                              ▼
                     [AI Interpretation]
                (Gemini API generates summary)
                              │
                              ▼
                        [Streamlit UI]
          (Interactive dashboard with insights & visuals)
```

---

## 🧠 **Setup & Installation**

### **1️⃣ Clone the repository**

```bash
git clone https://github.com/<your-username>/MedLens.git
cd MedLens
```

### **2️⃣ Create a virtual environment**

```bash
python -m venv venv
venv\Scripts\activate  # Windows
# or
source venv/bin/activate  # Mac/Linux
```

### **3️⃣ Install dependencies**

```bash
pip install -r requirements.txt
```

### **4️⃣ Add your API Key**

Create a `.env` file (or add in Streamlit secrets):

```
API_KEY = "your_gemini_api_key"
```

### **5️⃣ Run the app**

```bash
streamlit run app.py
```

App runs locally on 👉 `http://localhost:8501`

---

## 🌐 **Deployed Link**

🔗 [Live App] https://medlensbylynk-3v8sfnp9cicf7jthvwafwf.streamlit.app/

---







## 🚀 **Future Scope**
(Points in presentation)
* Integration with wearable health data (Fitbit, Apple Health).
* Multi-language medical interpretation.
* Doctor-mode dashboard with advanced analytics.
* Real-time anomaly detection via AI alerts.
* Voice-based medical report explanation (text-to-speech).

---

## 👩‍💻 **Team Members**

| Name         | Role                     |
| ------------ | ------------------------ |
| Kriti [You]  | AI & Backend Developer   |
| Kinjal Srivastava | Frontend & Design   |

---

## 🏁 **Commit History**

A clear and consistent commit trail has been maintained to show progressive development across:

* Phase 1: OCR Extraction
* Phase 2: AI Integration
* Phase 3: Visualization + Deployment

---

## 🩷 **Thank You**

> “Empowering users to understand their health — one report at a time.”

