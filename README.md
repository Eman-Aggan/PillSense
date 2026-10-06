# 💊 PillSense: Medicine Leaflet Assistant

An AI assistant that explains medicines in simple language, using answers grounded only in leaflet text.

## Problem
Medicine leaflets are long and full of jargon, and drug interactions are easy to miss.

## How it works
Photo or text → Gemini Vision reads the box → name normalized to the generic drug
(Panadol → paracetamol) → RAG retrieves relevant leaflet chunks → LLM answers
in English or Arabic using only that text.

## Tech stack
- Gemini (Vision + text generation)
- multilingual-e5 embeddings + FAISS (retrieval)
- Gradio (UI)
- Python, Google Colab

## Features
- Medicine recognition from a photo, brand name, or Arabic name
- Leaflet-grounded answers with cited sources
- Drug interaction questions
- Safe refusal when a drug isn't in the database

## Team
- Name 1: Vision & Data
- Name 2: RAG Engine
- Name 3: LLM & UI

## How to run
1. Open the notebook in Google Colab.
2. Add your Gemini API key in Colab Secrets as `GEMINI_API_KEY`.
3. Run all cells in order.

## Disclaimer
Educational project, not a substitute for a doctor or pharmacist.
The knowledge base contains simplified educational summaries, not official leaflets.
