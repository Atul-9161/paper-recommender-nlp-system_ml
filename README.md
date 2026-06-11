# Research Paper Recommender & Subject Classification System

An NLP-powered system that recommends semantically similar research papers and automatically predicts the subject area of a research paper using Deep Learning and Sentence Transformers.

## Demo

<p align="center">
  <img src="demo.gif" width="900">
</p>

> Add your recorded GIF as `demo.gif` in the repository root.

---

## Overview

This project combines **Semantic Search** and **Multi-Label Text Classification** to help researchers discover relevant academic papers and automatically categorize them into research domains.

The system provides:

* Research Paper Recommendation using Sentence Transformers
* Semantic Similarity Search with Cosine Similarity
* Multi-Label Subject Classification using Deep Learning
* Interactive Streamlit Web Interface

---

## Features

### Research Paper Recommendation

* Converts research paper text into semantic embeddings using Sentence Transformers.
* Computes cosine similarity between papers.
* Retrieves the Top-5 most relevant research papers.
* Supports semantic matching beyond simple keyword search.

### Subject Area Classification

* Processes research paper abstracts using NLP techniques.
* Uses a TensorFlow/Keras-based deep learning model.
* Predicts one or more subject areas from paper abstracts.

Example subject areas:

* Machine Learning
* Artificial Intelligence
* Natural Language Processing (NLP)
* Computer Vision
* Data Mining

---

## System Architecture

### Recommendation Pipeline

```text
Paper Title
     │
     ▼
Sentence Transformer
     │
     ▼
Vector Embedding
     │
     ▼
Cosine Similarity
     │
     ▼
Top-5 Recommended Papers
```

### Classification Pipeline

```text
Paper Abstract
      │
      ▼
TextVectorization
      │
      ▼
Deep Learning Model
      │
      ▼
Predicted Subject Areas
```

---

## Tech Stack

### Languages

* Python

### Machine Learning & NLP

* TensorFlow
* Keras
* Sentence Transformers
* Scikit-Learn
* NumPy

### Deep Learning

* Multi-Layer Perceptron (MLP)
* Text Embeddings
* Multi-Label Classification

### Deployment

* Streamlit

---

## Project Structure

```text
research-paper-recommender-ml/
│
├── app.py
├── requirements.txt
├── README.md
│
├── models/
│   ├── embeddings.pkl
│   ├── model.h5
│   ├── rec_model.pkl
│   ├── sentences.pkl
│   ├── text_vectorizer_config.pkl
│   ├── text_vectorizer_weights.pkl
│   └── vocab.pkl
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Atul-9161/paper-recommender-nlp-system_ml.git
cd paper-recommender-nlp-system_ml
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
streamlit run app.py
```

---

## Example

### Input Title

```text
Graph Neural Networks for Learning on Structured Data
```

### Output Recommendations

```text
1. A Generalization of Convolutional Neural Networks to Graph-Structured Data
2. Deep Loopy Neural Network Model for Graph Structured Data Representation Learning
3. IPC: A Benchmark Data Set for Learning with Graph-Structured Data
4. Deep Convolutional Networks on Graph-Structured Data
5. Learning Discrete Structures for Graph Neural Networks
```

---

## Future Improvements

* FAISS-based similarity search for faster retrieval.
* Transformer-based subject classifier (BERT/RoBERTa).
* Research paper PDF upload support.
* Research paper metadata filtering.
* Cloud deployment.

---

## Author

**Atul Mishra**

GitHub: https://github.com/Atul-9161

---

## License

This project is developed for educational and research purposes.

