# Groq Conversation Management & Classification

A comprehensive implementation of conversation management and information extraction using Groq API with OpenAI SDK compatibility.

## ⚠️ Security Note
**This repository contains an API key as per assignment requirements for testing purposes.**

- The API key is included specifically for assignment evaluation
- In production environments, API keys should NEVER be committed to version control
- This is a temporary key that will be revoked after evaluation
- I understand the security implications and have included it only to meet assignment requirements

*For real-world applications, I would use environment variables or secure key management services.*

## 🎯 Project Overview

This project implements two core functionalities:
1. **Conversation Management System** - Manages chat history with intelligent truncation and periodic summarization
2. **Information Extraction System** - Extracts structured user information from conversations using JSON schema

## 🚀 Features

### Task 1: Conversation Management
- **Flexible Truncation Options**:
  - Limit by number of conversation turns
  - Limit by character/word length
  - Combined truncation (turns + length)
- **Periodic Summarization**:
  - Automatic summarization every k conversations
  - Summary consolidation with previous summaries
  - Intelligent context preservation

### Task 2: Information Extraction
- **Structured Data Extraction** for 5 fields:
  - Name
  - Email
  - Phone
  - Location (city, state, country)
  - Age
- **JSON Schema Validation**
- **Function Calling** using Groq's OpenAI-compatible API
- **Flexible Extraction** from various conversation styles

## 🛠️ Technologies Used

- **API**: Groq API (OpenAI-compatible)
- **Model**: llama-3.1-8b-instant
- **Language**: Python 3.x
- **Libraries**: OpenAI Python SDK
- **Environment**: Google Colab

## 📋 Requirements

```bash
pip install openai


                
🔑 API Setup
The notebook includes a working API key for testing (as per assignment requirements)
For your own use, get an API key from console.groq.com
Replace the API key in the notebook with your own
📊 Results
Successfully implemented conversation truncation with 3 different methods
Periodic summarization tested with 6 conversations (2 summaries created)
Information extraction validated on 3 diverse conversation samples
100% validation success rate on all test cases
📝 Usage
Open the notebook in Google Colab
Run all cells sequentially
View demonstrations of both tasks
Modify parameters to test different scenarios
🎓 Assignment Context
This project was completed as part of an internship assignment that specifically required:

No frameworks (only standard Python + OpenAI client)
Groq API with OpenAI-compatible SDK
API keys included in the notebook for test runs
Clean, well-documented code
Comprehensive demonstrations
All requirements have been met while understanding security best practices for real-world applications.

📄 License
This project is created for educational purposes.

Author: Kunal Sharma
Date: September 25 2025
Note: API key included as per assignment requirements - will be revoked post-evaluation
