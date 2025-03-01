Project Description: AI-Powered Resume Screening and Job Matching System (Local Processing with Vector Database)
Overview
This project is a fully local AI-powered resume screening and job matching system that enables efficient retrieval of the most relevant resumes based on a given job description. It leverages FAISS, a vector database, for fast similarity search, SentenceTransformers for text embeddings, and PyPDF2 for extracting resume content.
Key Highlights:
•	No external API dependencies (works entirely offline).
•	Fast resume search using the FAISS vector database for efficient retrieval.
•	Local embedding model (all-MiniLM-L6-v2) ensures privacy-friendly text processing.
•	Handles multiple PDF resumes, extracting text and matching them to job descriptions.
Key Features
1.	Resume Upload & Text Extraction
o	Reads PDF resumes from a local folder.
o	Extracts text content using PyPDF2.
2.	Text Embedding & Vector Storage
o	Uses SentenceTransformers (all-MiniLM-L6-v2) to convert resumes into vector embeddings.
o	Stores the embeddings in FAISS, a high-performance vector database for similarity search.
3.	Resume Search & Matching
o	Accepts a job description as input.
o	Converts the job description into an embedding.
o	Uses FAISS vector database to retrieve the top resumes based on similarity search.
4.	Fully Local Processing with Vector Database
o	No API dependencies – all operations run on the local machine.
o	Ideal for privacy-sensitive applications where external cloud services are not permitted.
Tech Stack
•	Vector Database: FAISS (Facebook AI Similarity Search)
•	Embedding Model: SentenceTransformers (all-MiniLM-L6-v2)
•	PDF Processing: PyPDF2
•	Programming Language: Python
•	Framework: Jupyter Notebook
Workflow
1.	User places PDF resumes in the designated folder (resumes/).
2.	The system extracts text from the resumes.
3.	Embeddings are generated for each resume.
4.	Embeddings are stored and indexed in the FAISS vector database.
5.	User provides a job description for candidate matching.
6.	The system retrieves the top-matching resumes using vector similarity search from FAISS.
