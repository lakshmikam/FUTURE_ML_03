This project focuses on building an NLP-based resume screening system that automatically evaluates resumes against a given job description and ranks candidates based on relevance. The system simulates real-world Applicant Tracking Systems (ATS) used by recruitment platforms and HR-tech companies.

The solution processes unstructured resume data, extracts textual features, computes similarity scores, and identifies skill gaps to support recruiter decision-making.

Problem Statement

Recruiters often receive hundreds or thousands of resumes for a single job role. Manually reviewing each resume is inefficient and inconsistent.

This project aims to automate:

Resume parsing and text extraction

Resume-to-job similarity scoring

Candidate ranking based on relevance

Identification of missing or weak skills

The system demonstrates how Natural Language Processing can be applied to streamline hiring workflows.

Dataset

Dataset Used: Resume Dataset

Kaggle Link:
https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset

The dataset consists of multiple resumes organized by job categories. The resumes are stored as PDF files and were parsed using PyPDF2 for text extraction.

A custom job description was defined within the project to simulate real hiring requirements.

Methodology

The project follows a structured NLP pipeline:

Resume Parsing
PDF resumes were parsed using PyPDF2 to extract raw text content.

Text Preprocessing
Extracted text was cleaned and normalized for further processing.

Feature Extraction
TF-IDF vectorization was applied to convert resume text and job description into numerical representations.

Similarity Computation
Cosine similarity was used to measure the relevance between each resume and the job description.

Candidate Ranking
Resumes were ranked based on similarity scores, enabling automatic shortlisting.

Skill Gap Identification
The system dynamically compared resume content with job description keywords to identify missing skills.

Results

The system successfully ranked thousands of resumes based on job relevance and identified missing skills dynamically. The approach demonstrates how classical NLP techniques can be effectively used to build scalable resume screening systems.

The solution mirrors real-world resume filtering logic used in recruitment platforms.

Future Improvements

Potential enhancements include:

Implementing semantic embeddings for deeper contextual understanding

Introducing weighted skill importance

Deploying as a web-based screening dashboard

Adding database integration for candidate management
