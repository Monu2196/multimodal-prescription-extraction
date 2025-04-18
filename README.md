Multimodal LLM for Extracting Structured Data from Handwritten Medical Prescriptions

This project aims to extract structured information (like patient name, age, medicine name, dosage, duration) from scanned **handwritten medical prescriptions** using a **multimodal large language model (LLM)**.

---

Objective

To build an end-to-end pipeline using a multimodal LLM that takes an image of a handwritten prescription and outputs structured, machine-readable information.

---
Dataset

- **Name**: Medical Prescription Images Dataset  
- **Description**: A set of scanned handwritten medical prescriptions, annotated for fields such as:
  - Patient Name
  - Age / Sex
  - Medicines
  - Dosage
  - Duration
  - Instructions

---

Approach

We used a multimodal model (e.g., [Donut](https://github.com/clovaai/donut)) to process prescription images and directly generate structured output in JSON format.

The pipeline includes:
- Preprocessing images (resizing, normalization)
- Feeding images into the model
- Post-processing model output
- Evaluating extraction accuracy

---

Evaluation Strategy

Evaluation is based on:
- **Field-level accuracy**: how accurately each data field (e.g., medicine name, dosage) is extracted
- **Exact match score**: for JSON-based comparison
- **Manual review**: for low-confidence predictions and model interpretability

Scripts for evaluation are in the `evaluation/` folder.

---

## 🗂️ Project Structure

