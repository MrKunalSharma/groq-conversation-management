# Groq Conversation Management & Classification

A comprehensive implementation of conversation management and information extraction using the Groq API (OpenAI-compatible SDK).

## 🎯 Project Overview

This project implements two core functionalities:

1. **Conversation Management System** — Manages chat history with intelligent truncation and periodic summarization.
2. **Information Extraction System** — Extracts structured user information from conversations using a JSON schema.

## 🚀 Features

### Task 1: Conversation Management
- **Flexible truncation options**
  - Limit by number of conversation turns
  - Limit by character/word length
  - Combined truncation (turns + length)
- **Periodic summarization**
  - Automatic summarization every k conversations
  - Summary consolidation with previous summaries
  - Intelligent context preservation

### Task 2: Information Extraction
- **Structured data extraction** for 5 fields:
  - Name
  - Email
  - Phone
  - Location (city, state, country)
  - Age
- **JSON Schema validation**
- **Function calling** using Groq’s OpenAI-compatible API
- **Robust prompts** that handle varied conversation styles

## 🛠️ Tech Stack
- **API**: Groq API (OpenAI-compatible)
- **Model**: `llama-3.1-8b-instant`
- **Language**: Python 3.x
- **Library**: OpenAI Python SDK
- **Environment**: Google Colab (recommended)

## 📋 Requirements
- Python 3.10+
- OpenAI Python SDK

```bash
pip install openai
```

## 🔑 API Setup
- For evaluation, the notebook includes a working API key (as per assignment requirements).
- For personal use:
  - Get an API key from `https://console.groq.com`.
  - Replace the placeholder in the notebook with your own key.
- In production, use environment variables or a secure key manager; never commit API keys to version control.

## 🧪 Usage
- Open the notebook in Google Colab.
- Run cells sequentially to see:
  - Conversation truncation with three strategies
  - Periodic summarization
  - Information extraction and schema validation
- Adjust parameters to test different scenarios.

## 📊 Results
- Conversation truncation implemented with three different methods
- Periodic summarization tested with 6 conversations (2 summaries created)
- Information extraction validated on 3 diverse samples
- 100% validation success rate on all test cases

## ⚠️ Security Notice
This repository contains an API key strictly for assignment evaluation. The key will be revoked after evaluation. In real-world applications, API keys must never be committed; use environment variables or a secure key management service.

## 🎓 Assignment Context
This project was completed as part of an internship assignment with the following constraints:
- No frameworks beyond standard Python and the OpenAI client
- Use of the Groq API via the OpenAI-compatible SDK
- API key included in the notebook for test runs
- Clean, well-documented code with comprehensive demonstrations

All requirements have been met while acknowledging best practices for security.

## 📄 License
This project is created for educational purposes.

---
**Author**: Kunal Sharma  
**Date**: September 25, 2025  
**Note**: API key included as per assignment requirements; it will be revoked post-evaluation.
