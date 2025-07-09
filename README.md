# AI Chatbot using Gemini API and Transformers

## Problem Statement

Conventional chatbots often lack contextual awareness, memory retention, or intelligent similarity comparison between user inputs. This makes human-computer interaction rigid, repetitive, and less intuitive. There is also often no persistent conversation history or semantic understanding between sentences.

## Solution

This project implements a Python-based AI chatbot using Google's Gemini API and Transformer-based sentence embeddings (via Sentence-Transformers) to support:
- Conversational memory via history logging
- Semantic understanding using cosine similarity
- Contextual awareness for natural, human-like dialogue

By saving the full history of interactions and comparing input meanings with embeddings, the chatbot responds more intelligently and provides a more human experience.

## Features

- Integration with Gemini Pro (Flash) API for generating AI responses
- Transformer-powered sentence embedding with `all-MiniLM-L6-v2`
- Cosine similarity calculation to compare messages
- Automatic conversation history saved to `chat_history.txt`
- Virtual environment support for isolation
- Secure API key loading via `.env` file
- `.gitignore` configuration to protect sensitive files and environments

## Requirements

- Python 3.8+
- `requests`
- `python-dotenv`
- `sentence-transformers`
- `torch`

You can install dependencies using:

```bash
pip install -r requirements.txt