# Human-Centered HIV Drug Resistance Interpretation using MedGemma

This repository contains a **minimal, reproducible demonstration** of a human-centered
clinical decision-support application built for the **MedGemma Impact Challenge**.

The project combines:
- an HIV drug resistance **machine-learning model** (prediction), and
- a **HAI-DEF model from the MedGemma (Gemma-family) collection** (explanation).

The focus is on **responsible AI use**, interpretability, and safe communication.

---

## Overview

Machine-learning models can estimate HIV drug resistance risk from viral sequence–derived
features, but their outputs are often difficult to interpret and communicate safely.

This project demonstrates how **MedGemma (HAI-DEF)** models are used  
**not for prediction**, but for **human-centered explanation**:

- Clinician-facing explanations include uncertainty and limitations  
- Patient-facing explanations are carefully reviewed and **fixed (not generated live)**  

This system is **decision-support only** and does not provide diagnoses or treatment
recommendations.

---

## Repository structure
├── inference_demo.ipynb # End-to-end demo for one illustrative case
├── requirements.txt # Minimal Python dependencies
└── README.md

---

## How to run the demo

### Requirements
- Python 3.9+
- PyTorch
- Hugging Face Transformers
- GPU recommended (but not required for small examples)

### Install dependencies

```bash
pip install -r requirements.txt

-------------
Run the notebook

Open inference_demo.ipynb

Run all cells top to bottom

The notebook demonstrates:

An example output from an HIV drug resistance ML model

A clinician explanation generated using a MedGemma (HAI-DEF) instruction-tuned model

A frozen, patient-safe explanation printed as fixed text

Only a single illustrative case is used, as the hackathon does not provide an official dataset
and the focus is on application design and responsible model usage.
----------------------------------------
Notes on model access

MedGemma models are gated on Hugging Face.

To run the notebook end-to-end:

Accept the MedGemma / Gemma license on Hugging Face

Authenticate using a Hugging Face access token

If access is not available, the notebook still demonstrates correct MedGemma usage, and the
outputs shown are representative of MedGemma behavior.
----------------------------------------------
Safety and intended use

This project is for demonstration and research purposes only

It is not a diagnostic system

No treatment or drug selection advice is provided

All outputs explicitly communicate uncertainty

Patient-facing explanations are intentionally fixed to prevent unsafe variability

Use of MedGemma / Gemma-family models is subject to HAI-DEF Terms of Use.
----------------------------------------------------------------
## Competition context

This repository supports a submission to the **MedGemma Impact Challenge** on Kaggle.

The focus of the submission is on:
- Effective and appropriate use of **HAI-DEF models**
- Human-centered explanation design
- Ethical and safety-aware AI integration in healthcare workflows
