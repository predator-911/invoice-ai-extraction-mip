# Invoice Key-Value Information Extraction (MIP)

**Author:** Lakshya Kumar  
**Notebook:** `MIP.ipynb`  
**Assignment:** Automated Invoice Field Extraction (PDF/Image) using Donut & OCR  
**Date:** August 2025

---

## 📜 Overview

This repository contains a robust and scalable pipeline for extracting key-value information from invoices in PDF and image formats. The solution leverages the SOTA OCR-free vision-language model (Donut) alongside classical OCR fallback for maximum reliability and accuracy.

The notebook `MIP.ipynb` is fully annotated and Colab-ready, supporting single or multi-page documents, rapid extension to new fields, and efficient operation on GPU hardware.

---

## 🚀 Features

- **End-to-End Extraction:** Automatically retrieves invoice number, date, supplier, customer, totals, line items, and more.
- **Multi-Format Support:** Works with PDFs (multi-page) and images (PNG, JPG, JPEG).
- **Dual Extraction System:**  
  - Uses the Donut DocVQA model for advanced field parsing.
  - Falls back to OCR+regex for critical fields if AI extraction fails.
- **Highly Scalable:**  
  - Flexible dictionary-based extraction; add new fields in seconds.
  - Portable and easy to fine-tune for future requirements or new document formats.
- **Structured Output:** Exports per-document results in human- and machine-readable JSON for easy grading or automation.
- **Colab & GPU Ready:** Designed for Google Colab but easily runs in local Python/Jupyter environments.

---

---

## 🛠️ Requirements

- Google Colab (recommended) or Jupyter Notebook
- Python 3.8+
- GPU for fast inference (in Colab: Runtime > Change runtime type > GPU)
- Key packages are installed automatically at runtime (see notebook).

---

## 🧑‍💻 Usage Guide

1. **Open** the `MIP.ipynb` notebook in Google Colab.
2. **Run** all cells sequentially:
    - Installs dependencies and loads the model.
    - Prompts you to upload your invoice (PDF or image).
    - Processes each page, extracting all required fields.
3. **Download** the structured JSON result at the end.
4. **Customize fields:**  
   Edit the `fields_to_extract` dictionary to add or remove extracted fields as required by your use-case.

---

## 📈 Scalability

- To add new extraction fields: simply add another item/question in the extraction dictionary.
- To process large volumes or folders of invoices, wrap the core pipeline in a loop over your file list.
- The AI model (Donut) can be further fine-tuned for your organizational data if higher accuracy is required.

---

## 📗 Assignment Summary

This notebook fulfills all assignment requirements by:
- Performing automated field extraction on any invoice format.
- Providing reliable accuracy via modern AI and robust fallbacks.
- Allowing easy extension to new fields and layouts for future scalability.
- Delivering clean, professional outputs and clear explanations so anyone can understand and build upon the code.

---

## 🏷️ Credits

Developed by **Lakshya Kumar** as part of the Invoice Key-Value Extraction assignment.

---

> For questions or feedback, please open an issue or reach out via GitHub!


