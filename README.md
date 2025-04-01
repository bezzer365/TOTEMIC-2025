# Extracting Alloy Data from Scientific PDFs – TOTEMIC Training School - 2025

Welcome to the GitHub repository for the session at the TOTEMIC Training School 2025: "Tools for Energy Materials Modelling Acceleration" Training School on Extracting Alloy Data from PDF Files. This repository contains all the code, tools, and examples you’ll need to automatically extract alloy composition and phase information from scientific papers using Nougat and LLMs (LLaMA via Hugging Face Transformers). All steps are designed to be run on Google Colab, making use of its free GPU resources.

# 🧪 Extracting Alloy Data from Scientific PDFs – Training School

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/bezzer365/TOTEMIC-2025/blob/main/NLP_for_Materials.ipynb)

Welcome to the GitHub repository for our **Training School on Extracting Alloy Data from PDF Files**.  
This repository contains all the code, tools, and examples you'll need to **automatically extract alloy composition and phase information** from scientific papers using **Nougat** and **LLMs (LLaMA via Hugging Face Transformers)**. All steps are designed to be run on **Google Colab**, making use of its free GPU resources.

---

## 🎯 Aim

The goal of this session is to **demonstrate and walk through** an end-to-end workflow for:
- Converting academic papers in PDF format into markdown text
- Cleaning and preparing that text
- Extracting alloy and phase information using a large language model
- Reviewing and saving the extracted data

The training is designed for **both coders and non-coders**, with **interactive input boxes** provided to guide users through each step without needing to write code.

---

## ⚙️ Setup & Usage Guide

All steps are run on **Google Colab**. You do not need to install anything locally.

### 1. 📥 Download Papers
- A set of academic PDF papers is preloaded in this repository.
- You can add more if needed.

---

### 2. 📄 Convert PDF to Markdown Text
- **Install Nougat** from GitHub (an open-source OCR-based tool for PDF parsing).
- Run Nougat to convert PDFs to `.mmd` markdown files.
- **Preview extracted text** using `IPython.display`.
- Optional: Open `.mmd` in **Overleaf** for clearer formatting.

---

### 3. 🧹 Clean Raw Text
- **Remove unwanted sections** (e.g., acknowledgments, references).
- Optionally remove abstract and introduction.
- Re-preview `.mmd` file as above to confirm it's clean.

---

### 4. 🔐 Login to Hugging Face
- You'll be prompted to **enter your Hugging Face access token**.
- This is required to use the LLaMA model via the Transformers library.

---

### 5. 🧠 Install Transformers v4.49.0
- This specific version of Hugging Face Transformers is needed for compatibility.
- Runtime will **restart automatically** after installation.

---

### 6. 🧪 Extract Alloy and Phase Information
- Use a fine-tuned **LLaMA-based LLM** to extract structured data from `.mmd` files.
- The model:
  - Identifies alloy compositions
  - Extracts phase-related information
  - Cleans the output and saves it as `.json` files in an output folder

---

### 7. 🔎 Preview Extracted Data
- Load and display the structured JSON data of extracted alloy and phase information.
- Easy to review in table or dictionary format.

---

### 8. 🧼 Utilities (Optional)
If you run into memory or performance issues:
- **Free GPU Memory**: Clears unused variables and CUDA memory cache.
- **Clear Cache**: Choose to clean Hugging Face and/or PyTorch cache.

---

## 📁 Repository Contents
