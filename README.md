# Pariksha – Automated Descriptive Answer Evaluation System

Pariksha is a web-based examination platform that automates the evaluation of descriptive student answers using Natural Language Processing (NLP).

The system allows teachers to create classrooms, tests, questions, and reference answers. Students can attempt tests by uploading handwritten answer images. Google Cloud Vision OCR extracts the text from the submitted answers, after which NLP-based text similarity is used to compare the student's response with the reference answer and generate an automated score.

## 🚀 Features

- Teacher and student authentication
- Classroom creation and student enrollment
- Test and question creation
- Reference-answer based evaluation
- Handwritten answer image upload
- Optical Character Recognition (OCR)
- Text preprocessing and normalization
- TF-IDF based text vectorization
- Cosine similarity based answer comparison
- Automatic descriptive-answer scoring
- Student result and answer review
- Teacher-side student performance monitoring
- Manual score correction by teachers
- Django-based web interface

## 🧠 How the Evaluation Works

The answer evaluation pipeline follows these steps:

```text
Student submits answer image
            ↓
      Image Upload
            ↓
   Google Cloud Vision OCR
            ↓
   Extracted Answer Text
            ↓
    Text Preprocessing
            ↓
       TF-IDF Vectorization
            ↓
     Cosine Similarity
            ↓
 Comparison with Reference Answer
            ↓
       Score Generation
            ↓
       Result Display
