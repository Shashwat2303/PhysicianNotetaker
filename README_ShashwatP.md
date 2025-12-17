# 🩺 Physician Notetaker – Medical NLP Pipeline

## Overview
This project implements an end-to-end **Natural Language Processing (NLP) pipeline** for converting unstructured physician–patient conversations into structured clinical documentation. The system focuses on extracting medically relevant information, understanding patient intent and sentiment, and generating clinician-ready summaries and SOAP notes.

The objective is to demonstrate a **practical, model-driven approach** to medical text processing rather than a conceptual prototype.

---

## Core Capabilities
- **Medical Named Entity Recognition (NER)**  
  Extracts clinically relevant entities such as symptoms, events, and temporal references.

- **Structured Clinical Summarization**  
  Converts free-form conversation text into concise, structured medical summaries.

- **Patient Sentiment & Intent Detection**  
  Identifies emotional state and primary intent using transformer-based inference.

- **Keyword Extraction**  
  Highlights clinically important terms to support fast review.

- **SOAP Note Generation** *(Bonus)*  
  Produces Subjective, Objective, Assessment, and Plan–style documentation directly from dialogue.

---

## Pipeline Architecture
1. Raw conversation input  
2. Entity extraction using pretrained NER models  
3. Sentiment and intent inference using transformer classifiers  
4. Model-driven summarization of medical context  
5. SOAP note generation via controlled prompting  
6. Validation and confidence-based warning checks  

Each stage is modular and can be independently improved, fine-tuned, or replaced.

---

## Tech Stack
- **Python**
- **spaCy**
- **HuggingFace Transformers**
- **KeyBERT**
- **Jupyter Notebook**

---

## How to Run
1. Open `Physician_Notetaker.ipynb`
2. Install required dependencies listed in the notebook
3. Run the cells sequentially to execute the full pipeline

All outputs are generated dynamically by models; no static or hard-coded summaries are used.

---

## Design Decisions
- Model-driven outputs to avoid brittle rule-only systems  
- Hybrid ML + lightweight validation for robustness  
- Structured JSON outputs to support EMR/EHR integration  
- Modular design for easy extension and deployment  

---

## Limitations
- Models are not fine-tuned on proprietary clinical datasets  
- Evaluation is qualitative due to lack of labeled ground truth  
- Real-time transcription integration is not included  

---

## Future Improvements
- Fine-tuning with clinical models (BioBERT, ClinicalBERT)
- Quantitative evaluation metrics for entity extraction
- Confidence scoring per extracted field
- Real-time speech-to-text integration
- Backend service deployment for clinical applications

---

**Prepared for:** Emitrr  
**Role:** AI Engineer Intern
