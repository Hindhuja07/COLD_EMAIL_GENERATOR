# COLD_EMAIL_GENERATOR
AI Resume-Based Cold Email Generator

An AI-powered application that generates personalized cold emails by analyzing a candidate’s resume and matching it with a job description. The system runs fully locally using Ollama and does not rely on external APIs.

Overview

This project automates the process of drafting tailored job application emails. It extracts key information from a candidate’s resume, aligns it with the provided job description, and generates a concise, professional cold email using a locally hosted language model.

The system is designed with performance optimization in mind, using structured parsing techniques and minimizing LLM calls.

Key Features

PDF resume upload and text extraction

Programmatic extraction of candidate details (name, email, skills)

Job description alignment

Dynamic cold email generation

Tone customization

Fully local LLM execution (Ollama)

Single model-call architecture for performance efficiency

Architecture

Resume text is extracted using PyPDF2.

Candidate details are parsed using regex and keyword detection.

Job description is truncated and structured.

A single optimized prompt is constructed.

Ollama (mistral model) generates the personalized email.

This design ensures:

Reduced latency

Lower token consumption

Stability without external dependencies

Technology Stack

Python

Streamlit

Ollama (mistral)

PyPDF2

Requests

Regular Expressions

Prompt Engineering

Installation
1. Install Ollama

Download from:
https://ollama.com

2. Pull Model
ollama pull mistral

3. Start Ollama
ollama serve

4. Install Dependencies
python -m pip install -r requirements.txt

5. Run Application
python -m streamlit run app.py


Open in browser:
http://localhost:8501

Project Structure
app.py
email_engine.py
requirements.txt
README.md
LICENSE

Intended Use

This tool is designed for:

Entry-level job applicants

Internship candidates

Graduates seeking structured outreach emails

Resume-driven job applications
