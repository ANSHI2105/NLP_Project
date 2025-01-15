# Automated Student Response Evaluation System

## Description
This project is an **NLP-based Automated Student Response Evaluation System** aimed at processing handwritten and textual student responses. It uses OCR tools to extract textual data and mathematical expressions, preprocesses the extracted content, and performs semantic similarity analysis against correct answers provided by teachers. The system provides automated grading by leveraging embedding techniques and similarity metrics, achieving a balance between accuracy and scalability in educational settings.

---

## Overview
This project involves developing a **Natural Language Processing (NLP)** system designed to evaluate student responses by comparing them with the correct answers provided by teachers. The primary goal is to extract text from student responses, preprocess it for semantic analysis, and calculate similarity scores to provide automated grading.

---

## Key Features

### Text Extraction:
- Utilized **Pytesseract** to extract textual data from handwritten student responses.
- Incorporated **Latex OCR** to detect and process complex mathematical expressions into LaTeX format.

### Text Processing:
- Preprocessed extracted text with techniques like:
  - Tokenization
  - Stop-word removal
  - Lemmatization
- Combined outputs from OCR tools into coherent text representations.

### Semantic Analysis:
- Leveraged NLP embedding techniques, including:
  - **TF-IDF Vectorization**
  - **Word2Vec**
  - **Doc2Vec**
  - **BERT-based model**
- Used **Cosine Similarity** and **Euclidean Distance** to evaluate the semantic relevance between student responses and correct answers.

### Scoring System:
- Automated grading system calculates similarity scores for each student response based on the correct answer, ensuring objective evaluation.

---

## Workflow

1. **Input Handling:**
   - Process student responses provided as images or text files.
   - Extract text and mathematical expressions using OCR tools.

2. **Text Preprocessing:**
   - Clean and tokenize extracted text to ensure compatibility with embedding techniques.

3. **Semantic Similarity Analysis:**
   - Apply embedding models to represent text in vector format.
   - Compute similarity scores using Cosine Similarity and Euclidean Distance.

4. **Automated Grading:**
   - Generate similarity scores and annotate student responses with feedback.

---

## Dependencies

### NLP Libraries:
- **NLTK**
- **Transformers**

### OCR Tools:
- **Pytesseract**
- **Latex OCR**

### Similarity Calculation:
- **Scikit-learn**

---

## Use Cases
- Automated grading of student responses in educational institutions.
- Semantic and contextual evaluation of handwritten and textual answers.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-repo>/student-response-evaluation.git
   cd student-response-evaluation
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the script:
   ```bash
   python main.py
   ```

---

## Usage

1. Place student responses in the `input/` directory.
2. Provide correct answers in the `correct_answers.json` file.
3. Run the script to evaluate responses and generate scores in the `output/` directory.

---

## Results
- Achieved **70% accuracy** in semantic similarity evaluation.
- Successfully processed **2000+ student responses** for automated grading.

---

## Future Work
1. Enhance model performance by fine-tuning domain-specific embeddings.
2. Incorporate multilingual support for broader applicability.

---

## Acknowledgments
Special thanks to Vignam Pvt. Ltd. for providing mentorship and resources to complete this project.

