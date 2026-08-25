# MAYA-AI-Women-Safety
# 🛡️ MAYA AI — Women Safety Assistant

<p align="center">
  <img src="assets/maya.png" width="900">
</p>

<h2 align="center">Your AI Companion for Safety & Empowerment</h2>

<p align="center">
  An AI-powered women safety assistant designed to understand safety-related conversations,
  classify risk levels, identify situations, and provide intelligent safety-oriented assistance.
</p>

<p align="center">

![Python](https://img.shields.io/badge/Python-3.x-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-ML-orange)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![Status](https://img.shields.io/badge/Status-In%20Development-purple)

</p>

---

## 🌸 About MAYA

**MAYA** is an AI-powered safety assistant created to help users communicate about potentially unsafe situations.

The system uses Natural Language Processing and Transformer-based machine learning models to analyze a user's message and determine:

- 🚨 **Risk Level**
- 🔎 **Situation Type**
- 💬 **Appropriate Safety Response**

The long-term goal is to integrate MAYA into a web and mobile safety platform.

---

# 🧠 AI Architecture

```text
                         USER
                          │
                          ▼
                   ┌─────────────┐
                   │ MAYA CHATBOT│
                   └──────┬──────┘
                          │
                          ▼
                    USER MESSAGE
                          │
              ┌───────────┴───────────┐
              │                       │
              ▼                       ▼
      ┌────────────────┐      ┌──────────────────┐
      │  RISK MODEL    │      │ SITUATION MODEL  │
      └───────┬────────┘      └────────┬─────────┘
              │                        │
              ▼                        ▼
       LOW / MEDIUM /            SITUATION TYPE
       HIGH / CRITICAL
              │                        │
              └───────────┬────────────┘
                          │
                          ▼
                  ┌───────────────┐
                  │ SAFETY ENGINE │
                  └───────┬───────┘
                          │
                          ▼
                    MAYA RESPONSE
                          │
                          ▼
                     USER / WEB
```

---

# 🤖 AI Models

## Model 1 — Risk Classification

The first model determines the potential severity of a user's message.

### Classes

```text
LOW
MEDIUM
HIGH
CRITICAL
```

### Example

```text
User:
"Someone has been following me."

        ↓

Risk Model

        ↓

HIGH
```

---

## Model 2 — Situation Classification

The second model identifies the type of situation described by the user.

```text
User Message
      ↓
Situation Model
      ↓
Situation Category
```

This allows MAYA to distinguish between different types of safety-related situations.

---

# 📊 Model Performance

### Current Test Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Risk Classifier | **100%*** | **100%*** | **100%*** | **100%*** |
| Situation Classifier | **100%*** | **100%*** | **100%*** | **100%*** |

> **Note:** These scores represent the current evaluation on the project's test datasets. They should not be interpreted as guaranteed real-world accuracy. Independent validation using completely unseen and representative data is required before deployment.

---

# 🛠️ Technologies Used

### Machine Learning

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Scikit-learn

### Development

- Google Colab
- FastAPI
- HTML
- CSS
- JavaScript

### Model Architecture

- DistilBERT
- Transformer-based text classification

---

# 📁 Project Structure

```text
MAYA-AI-Women-Safety/
│
├── assets/
│   └── maya-preview.png
│
├── models/
│   ├── maya_risk_model.zip
│   └── maya_situation_model.zip
│
├── notebooks/
│   └── MAYA_AI_TRAINING.ipynb
│
├── src/
│   ├── risk_prediction.py
│   ├── situation_prediction.py
│   └── maya_engine.py
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 💬 Example

### User

```text
Someone has been following me since I left work.
```

### MAYA AI

```text
Risk Level: HIGH

Situation: Potential stalking

Recommended Action:
Move toward a safe/public location and consider contacting
a trusted person or appropriate emergency assistance.
```

---

# 🚀 Development Roadmap

## ✅ Completed

- [x] Dataset preparation
- [x] Risk classification model
- [x] Situation classification model
- [x] Model evaluation
- [x] Model saving
- [x] Model download
- [x] GitHub project setup

## 🔄 In Development

- [ ] MAYA chatbot backend
- [ ] FastAPI integration
- [ ] Website integration
- [ ] Real-time message analysis
- [ ] Safety response engine

## 🔮 Future Features

- [ ] Voice-enabled MAYA
- [ ] Multilingual support
- [ ] Mobile application
- [ ] Location sharing
- [ ] Trusted contact system
- [ ] Emergency assistance workflow
- [ ] Real-time safety alerts
- [ ] Personalized safety recommendations
- [ ] Improved independent evaluation dataset

---

# 🔐 Safety Architecture

MAYA is designed so that AI predictions do **not independently trigger emergency actions**.

A safer architecture is:

```text
AI Detection
     ↓
Safety Engine
     ↓
User Confirmation
     ↓
Application Action
```

Emergency actions such as SOS, location sharing, or contacting a trusted person should be controlled by deterministic application logic and appropriate user confirmation.

---

# ⚠️ Disclaimer

MAYA AI is an experimental AI-assisted safety project.

The system may make incorrect predictions and should not be considered a replacement for:

- Emergency services
- Law enforcement
- Trusted contacts
- Professional support
- Personal safety judgment

Always follow appropriate local emergency procedures when there is immediate danger.

---

# 📚 Training

The models were trained using Google Colab with Transformer-based text classification.

The training notebook is available in:

```text
notebooks/MAYA_AI_TRAINING.ipynb
```

The trained models are available in:

```text
models/
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/MAYA-AI-Women-Safety.git
```

Enter the project:

```bash
cd MAYA-AI-Women-Safety
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it on macOS/Linux:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# 🌐 Planned API Architecture

```text
MAYA Website
     │
     ▼
Chat Interface
     │
     ▼
FastAPI Backend
     │
     ├───────────────┐
     ▼               ▼
Risk Model     Situation Model
     │               │
     └───────┬───────┘
             ▼
       Safety Engine
             │
             ▼
       MAYA Response
```

---

# 👩‍💻 Project Vision

> **Technology should not only be intelligent — it should make people feel safer, more informed, and more empowered.**

MAYA aims to combine artificial intelligence, conversational interfaces, and safety-focused application design to create a smarter digital companion for women's safety.

---

## ⭐ Project Status

**MAYA AI — Women Safety Assistant**

```text
Machine Learning        ████████████████████  100%
Model Training          ████████████████████  100%
Model Evaluation        ████████████████████  100%
Backend Integration     ███████░░░░░░░░░░░░░  In Progress
Website Integration     █████░░░░░░░░░░░░░░░  In Progress
```

---

<p align="center">

### 🛡️ MAYA AI

**Where Intelligence Meets Safety**

</p>
