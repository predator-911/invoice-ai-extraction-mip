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

## 🗂️ File Structure

