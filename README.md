# Textify-GPU

## Overview
Textify-GPU is a high-performance **Optical Character Recognition (OCR)** tool designed to extract text from images, whether handwritten or printed. By leveraging GPU acceleration, it ensures rapid processing while maintaining efficiency in storage usage. The system supports various file formats, allowing users to download extracted text as **DOCX, PDF, or TXT**. Its transformer-based model enhances accuracy, making it a reliable solution for text recognition.  

In addition to extracting raw text, Textify-GPU integrates AI-powered post-processing using **Groq API (llama-3.3-70b-versatile)** to refine the output. This ensures better text formatting and readability, making it ideal for various applications, from digitizing documents to automating data extraction.

---

## Features
- **Handwritten & Printed Text Extraction**: Supports both handwritten and printed text recognition.
- **Fast Processing**: Utilizes GPU computation for high-speed OCR.
- **Multiple Output Formats**: Extracted text can be downloaded as **DOCX, PDF, or TXT**.
- **Transformer-Based Model**: Uses `stepfun-ai/GOT-OCR2_0`, a cutting-edge transformer-based OCR model.
- **Post-Processing with AI**: Enhances extracted text using **Groq API** with `llama-3.3-70b-versatile` for improved accuracy and formatting.

---

## Model Details
- **OCR Model:** [stepfun-ai/GOT-OCR2_0](https://huggingface.co/stepfun-ai/GOT-OCR2_0)
- **Post-Processing API:** [Groq API](https://console.groq.com/keys) using `llama-3.3-70b-versatile` 

---


