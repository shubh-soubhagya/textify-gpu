# Textify-GPU

## Overview
Textify-GPU is a high-performance **Optical Character Recognition (OCR)** tool designed to extract text from images, whether handwritten or printed. By leveraging GPU acceleration, it ensures rapid processing while maintaining efficiency in storage usage. The system supports various file formats, allowing users to download extracted text as **DOCX, PDF, or TXT**. Its transformer-based model enhances accuracy, making it a reliable solution for text recognition.  

In addition to extracting raw text, Textify-GPU integrates AI-powered post-processing using **Groq API (llama-3.3-70b-versatile)** to refine the output. This ensures better text formatting and readability, making it ideal for various applications, from digitizing documents to automating data extraction.

---

## Google Colaboratory Link: [https://colab.research.google.com/drive/18pKBXhJ3O0I9euWq7IW9dyyVoLPTSRuJ?usp=sharing](https://colab.research.google.com/drive/18pKBXhJ3O0I9euWq7IW9dyyVoLPTSRuJ?usp=sharing)

The tool is developed in Google Colab as the model requires high computational power. However, if your local system supports it, you can run the provided `OCR_script.ipynb` file from the repository.

***📌 Note:***  
- **Use a high-resolution or scanned image as input.**  
- **Ensure that a T4 GPU is connected.**  


---

## Features
- **Handwritten & Printed Text Extraction**: Supports both handwritten and printed text recognition.
- **Fast Processing**: Utilizes GPU computation for high-speed OCR.
- **Multiple Output Formats**: Extracted text can be downloaded as **DOCX, PDF, or TXT**.
- **Transformer-Based Model**: Uses `stepfun-ai/GOT-OCR2_0`, a cutting-edge transformer-based OCR model.
- **Post-Processing with AI**: Enhances extracted text using **Groq API** with `llama-3.3-70b-versatile` for improved accuracy and formatting.

---

## Python Libraries Used
- `pyspellchecker` : Used for correcting spelling errors in extracted text while preserving structure.
- `transformers` :  Utilized for loading the OCR model (GOT-OCR2_0) to process images and extract text.
- `groq` : Calls Groq's `llama-3.3-70b-versatile` model API to clean and refine extracted text.
- `ipywidgets` : Builds the interactive GUI for uploading images and downloading extracted text.
- `pillow` :  Handles image processing, including opening and displaying uploaded images.
- `python-docx` :  Saves extracted text as a `.docx` document.
- `fpdf` : Converts extracted text into a formatted `.pdf` document.
- `re` : Uses regular expressions to add spaces after punctuation for better readability.
- `IPython` : Displays HTML elements for image previews and download links.
- `base64` : Encodes images and files for web display and downloads.
- `io` : Manages file streams for reading and writing images and text files.

The libraries `tiktoken`, `verovio`, and `indexer` are dependencies required for the **GOT-OCR2_0** model to function properly.


---
## Model Details
- **OCR Model:** [stepfun-ai/GOT-OCR2_0](https://huggingface.co/stepfun-ai/GOT-OCR2_0)
- **Post-Processing API:** [Groq API](https://console.groq.com/keys) using `llama-3.3-70b-versatile` 

---


