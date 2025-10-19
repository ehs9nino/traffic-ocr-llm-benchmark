# Traffic OCR–LLM Benchmark Dataset
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17392715.svg)](https://doi.org/10.5281/zenodo.17392715)


This repository contains two datasets used in the study:

**"Traffic Document Processing with Large Language Models:  
A Benchmark for Information Extraction from Noisy OCR" (Qader et al., 2025, PeerJ Computer Science)**

---

## 📁 Dataset Overview

### 1. Rate Confirmation Documents
- **15** synthetic rate confirmation images (`a1.jpg`–`a15.jpg`)
- Ground truth provided in `ratecon_ground_truth.json`
- Each record includes:
  - Load Number  
  - Pickup / Dropoff Location and Time  
  - Total Rate and Rate per Mile  

These images are **synthetic and anonymized**, suitable for both:
- **OCR + LLM vision–text benchmarking**
- **Text-only information extraction** after OCR

---

### 2. Driver / CDL Documents
- **40** pseudonymized driver license entries  
- Files:
  - `drivers_all_40_pseudomised_manually.json` – ground truth key–value pairs  
  - `ocr_drivers_combined_pseudonymized.csv` – OCR text outputs  
  - `driver1.jpg`–`driver4.jpg` – blurred, anonymized samples  

Due to privacy and ethical considerations, **the original driver images are not included**.  
These documents were derived from real-world samples but carefully **pseudonymized** to remove all personal identifiers.  
This subset is therefore suitable for **text-based LLM benchmarking only** (no vision inputs).

---

## 🔒 Data Ethics and Privacy

All datasets included in this repository comply with ethical research standards and data protection principles:
- No personally identifiable information (PII) is present.  
- Driver license data have been manually pseudonymized.  
- Rate confirmation samples are fully synthetic or anonymized.  
- This dataset must **not** be used for any form of biometric or identity reconstruction.  

By using this dataset, you agree to respect these conditions.

---

## 🧠 Usage Notes

- The **Rate Confirmation subset** can be used for full OCR + LLM pipeline evaluation (vision or text-based).  
- The **Driver / CDL subset** is limited to text-based or OCR-output evaluation only.  
- Combining both allows benchmarking of **cross-domain document understanding** tasks.

---

## ⚖️ License

This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.  
You are free to share and adapt the data, provided that appropriate credit is given to the authors.  
Do not attempt re-identification or reconstruction of personal data.

---

## 📜 Citation

Ehsan Qader, Dmitry Efremenko, Denis Derkach (2025).  
*Traffic Document Processing with Large Language Models:  
A Benchmark for Information Extraction from Noisy OCR.*  
PeerJ Computer Science.

---

## 📬 Contact

For dataset-related inquiries, please contact:  
**Ehsan Qader** — [GitHub Issues](https://github.com/ehs9nino/traffic-ocr-llm-benchmark/issues)
