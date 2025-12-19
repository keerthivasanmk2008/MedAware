# MedAware

# 👁️ EyeScan AI – Multimodal Health Screening System

EyeScan AI is a **web-based AI health screening application** that analyzes **eye images, text symptoms, and voice input** to provide **preliminary medical insights**.  
The system combines **CNN-based image analysis** with **Google Gemini’s multimodal AI reasoning** to generate structured health reports with risk evaluation.

> ⚠️ This tool is for **educational and screening purposes only** and is **not a replacement for professional medical diagnosis**.

---

## 🚀 Features

- 📸 **Eye Image Screening (CNN-based)**
- 📝 **Text Symptom Analysis**
- 🎙 **Voice-Based Symptom Input**
- 🧠 **AI-Generated Health Summary**
- 📊 **Severity / Risk Scoring (Low–Medium–High)**
- 🔐 **User Authentication (Firebase)**
- 🌐 **Fully Web-Based (No installation needed)**

---

## 🧠 AI & ML Models Used

### 🔹 1. Convolutional Neural Network (CNN)
- Used for **eye image analysis**
- Extracts visual features such as:
  - Redness
  - Texture changes
  - Abnormal regions
- Implemented via a **custom-trained CNN model hosted on Hugging Face**
- Acts as the **primary vision model**

### 🔹 2. Google Gemini (Multimodal LLM)
- Used for:
  - Medical reasoning
  - Text & voice symptom understanding
  - Report generation
- Models used:
  - `gemini-3-flash-preview`
  - `gemini-2.5-flash`
  - `gemini-2.0-flash`
- Works as a **fallback for vision analysis** if CNN is unavailable

### 🔹 3. Hybrid AI Architecture
| Component | AI Technique |
|--------|-------------|
| Eye Image | CNN (Deep Learning) |
| Text Symptoms | NLP (LLM) |
| Voice Input | Speech Recognition + NLP |
| Diagnosis Logic | Prompt-engineered AI reasoning |
| Risk Level | Rule-based scoring |

---

## 🧩 Algorithm Workflow

1. **Input Collection**
   - Image / Text / Voice
2. **Preprocessing**
   - Image → Base64
   - Voice → Text (Web Speech API)
3. **CNN Feature Extraction**
   - Eye image analyzed using CNN
4. **AI Reasoning**
   - Gemini generates diagnosis & advice
5. **Risk Evaluation**
   - Severity score (0–100)
6. **Result Visualization**
   - Condition, symptoms, precautions, diet, confidence bar

---

## 🛠 Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript (ES6)
- Lucide Icons

### AI / ML
- CNN (Hugging Face deployment)
- Google Gemini API (Multimodal LLM)

### APIs & Services
- Firebase Authentication
- Hugging Face Spaces
- Web Speech API
- MediaDevices API (Camera)

---

