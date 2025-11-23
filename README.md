# CENG 543 - Information Retrieval: Midterm Examination Project

**Student Name:** Furkan KARA

**Student Email:** furkankara@std.iyte.edu.tr

**Student ID:** 300201046

**Course:** CENG 543 - Information Retrieval (Prof. Dr. Aytuğ Onan)

---

## Project Overview
This project contains the solutions for the Take-Home Midterm Examination. The work explores various deep learning architectures for NLP, including RNNs, Attention Mechanisms, Transformers, RAG systems, and Interpretability methods.

## Folder Structure
The submission archive is organized as follows:

* **`Code/`**: Contains 5 Jupyter Notebooks (.ipynb), one for each exam question.
    * `Q1_Sentiment_Analysis.ipynb`: Comparative analysis of Bi-LSTM/Bi-GRU with GloVe & BERT.
    * `Q2_Machine_Translation.ipynb`: Seq2Seq models with Additive, Multiplicative, and Dot-Product Attention.
    * `Q3_Transformer.ipynb`: Transition from RNN to Transformer architecture (Translation task).
    * `Q4_RAG_System.ipynb`: Retrieval-Augmented Generation using BM25 and FLAN-T5.
    * `Q5_Interpretability.ipynb`: Model interpretability using Captum (Integrated Gradients).
* **`Report/`**: Contains the detailed project report in PDF format (LaTeX generated).
* **`Data/`**: This folder is left empty to minimize file size. The code is designed to automatically download necessary datasets (IMDb, Multi30k, SQuAD) and embeddings (GloVe) upon execution.
* **`Models/`**: This folder is left empty. Models are trained during the execution of the notebooks.

---

## How to Run the Code

### 1. Prerequisites
The project requires Python 3.x and PyTorch. You can install all necessary dependencies using the `requirements.txt` file provided in the root directory.

```bash
pip install -r requirements.txt

2. Execution Order
It is recommended to run the notebooks in the following order, although they can run independently:

Code/Q1_Sentiment_Analysis.ipynb

Code/Q2_Machine_Translation.ipynb

Code/Q3_Transformer.ipynb

Code/Q4_RAG_System.ipynb

Code/Q5_Interpretability.ipynb

3. Runtime Environment
Google Colab (Recommended): These notebooks were developed and tested on Google Colab. It is highly recommended to run them on Colab using a T4 GPU runtime for faster training, especially for Question 3 (Transformer) and Question 1 (BERT).

Local Machine: If running locally, ensure you have CUDA installed if you wish to utilize GPU acceleration.

Important Notes
Data Download: The script !wget (for GloVe) and Hugging Face datasets library are used to fetch data. Please ensure an active internet connection when running the cells for the first time.

Training Time: Transformer models (Q3) may take some time to train depending on the hardware. The notebooks include "Quick Test" parameters (commented out or set as default) to demonstrate functionality without long wait times.