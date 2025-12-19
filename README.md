# xai_brain_stroke
## ⚠️ Disclaimer
This project is for **research and educational purposes only** and is **not a replacement for professional medical diagnosis**.
# XAI-Driven Brain Stroke Detection with Agentic AI and Multimodal LLM Reporting

## 📌 Overview
This project presents an end-to-end AI-driven framework for automated **brain stroke detection from non-contrast CT scans**, enhanced with **Explainable AI (XAI)**, **ensemble learning**, and **multimodal Large Language Model (LLM)-based clinical report generation**.

Unlike traditional black-box classifiers, this system focuses on **clinical interpretability, reliability, and decision support**, making it suitable for real-world medical imaging workflows.

---

## 🚀 Key Features
- 🧠 **Stroke Detection from CT Scans**
- 🤖 **Three Deep Learning Models**
  - Custom CNN
  - ResNet18
  - AlexNet
- 🔍 **Explainable AI (XAI)**
  - Grad-CAM visualizations for each model
- 🧩 **Agentic AI Framework**
  - Ensemble majority voting
  - Confidence scoring for predictions
- 📝 **Automated Clinical Report Generation**
  - Multimodal LLM (Llama-3-Vision via Groq API)
  - Generates structured radiology-style reports:
    - Findings
    - Impression
    - Recommendations

---

## 🏗️ System Architecture
1. Input Brain CT Scan  
2. Parallel inference using CNN, ResNet18, and AlexNet  
3. Grad-CAM heatmap generation for each model  
4. Agentic AI module:
   - Aggregates predictions
   - Computes confidence score
5. Multimodal LLM analyzes:
   - CT image
   - Grad-CAM heatmaps
   - Ensemble output
6. Automated clinical report generation  

---

## 📂 Dataset
- **Brain Stroke CT Dataset**
- Binary classification: `Stroke` vs `Non-Stroke`
- Data split into:
  - Training
  - Validation
  - External test set

---

## 🧠 Model Performance

| Model        | Accuracy | Precision | Recall | F1-Score |
|-------------|----------|-----------|--------|----------|
| Custom CNN  | 92.5%    | 0.91      | 0.93   | 0.92     |
| AlexNet    | 93.8%    | 0.92      | 0.94   | 0.93     |
| ResNet18   | **95.3%**| **0.94**  | **0.96** | **0.95** |

ResNet18 demonstrated the best balance between **accuracy, recall, and explainability**.

---

## 🔍 Explainable AI (Grad-CAM)
- Highlights clinically relevant regions:
  - Ischemic hypoattenuation
  - Hemorrhagic hyperdense areas
- Improves trust and transparency
- Enables visual validation of model reasoning

---

## 🤖 Agentic AI Module
- Uses **majority voting** across models
- Computes confidence score:
- Confidence = (Votes for majority class / 3) × 100  

- Flags low-confidence cases for human review

---

## 📝 Automated Clinical Report Generation
- Multimodal LLM processes:
- CT scan
- Grad-CAM heatmaps
- Model predictions
- Outputs a structured radiology-style report:
- Findings
- Impression
- Recommendations

This transforms the system from a classifier into a **semi-automated diagnostic assistant**.

---

## 🛠️ Tech Stack
- **Programming:** Python  
- **Deep Learning:** PyTorch  
- **Models:** CNN, ResNet18, AlexNet  
- **XAI:** Grad-CAM  
- **Agentic AI:** Ensemble + confidence scoring  
- **LLM:** Llama-3-Vision (Groq API)  

---

## 📌 Future Enhancements
- Multi-center and multi-modal datasets (CTA, MRI)
- Transformer / ViT-based architectures
- PACS and hospital workflow integration
- Prospective clinical validation

---

## 📄 Publication
**"XAI-Driven Stroke Detection from Brain CT Images using Agentic AI and Multimodal LLMs"**  
Accepted for academic publication.

---

## 👨‍💻 Authors
- Gautam Kumar  
- Sayed Sajid Ali  
- Gitanshu Choudhary  
- Anuja Kumar Acharya  

---


