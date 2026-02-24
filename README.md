# Human-Centered HIV Drug Resistance Interpretation using MedGemma

This repository contains a **minimal, reproducible demonstration** of a human-centered
clinical decision-support application built for the **MedGemma Impact Challenge**.

The project combines:
- an HIV drug resistance machine-learning model (prediction), and
- a **HAI-DEF language model from the Gemma / MedGemma family** (explanation).

The focus is on **responsible AI use**, interpretability, and safe communication.

---

## Overview

Machine-learning models can estimate HIV drug resistance risk from viral sequence–derived features,
but their outputs are often difficult to interpret and communicate safely.

This project demonstrates how **MedGemma / Gemma-family HAI-DEF models** can be used
*not for prediction*, but for **human-centered explanation**:
- Clinician-facing explanations include uncertainty and limitations
- Patient-facing explanations are carefully reviewed and **fixed (not generated live)**

This system is **decision-support only** and does not provide diagnoses or treatment recommendations.

---

## Repository structure
