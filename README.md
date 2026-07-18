# NLP-Based Medical Diagnosis Assistant Chatbot

This project is an intelligent, conversational medical guidance application developed as a practical project within the **Project Development in Python** curriculum, a component of the **Microsoft Python Development Professional Certificate** program on Coursera. The system processes user-reported health symptoms, executes tokenization pipelines, matches entities against a structured medical knowledge base, applies multi-turn conversational loops, and delivers non-diagnostic clinical advice and emergency warnings based on structured data vectors.

---

## Technical Specifications and Scope

### Academic and Professional Credential Context
* Certification Program: Microsoft Python Development Professional Certificate
* Platform Provider: Coursera
* Course Focus: Project Development in Python, Natural Language Processing, and Conversational Logic

### Natural Language Processing and Chatbot Logic
* NLP Framework Engine: spaCy core architecture running the `en_core_web_sm` English linguistic pipelines
* Tokenization Pipeline: Iterates through discrete textual token objects via doc strings to extract raw linguistic text attributes
* Linguistic Normalization: Implements token lowercase conversion protocols using string methods to eliminate classification mismatches
* Rule-Based Entity Matching: Executes automated array membership operations using conditional membership filters to parse isolated words against target medical arrays

### Algorithmic Processing and Response Optimization
* Scoring Matrix Sorting: Implements advanced lambda key functions inside Python sorting methods (`sorted()`) to order matching health conditions in descending order based on localized statistical symptom weights
* Multi-Turn Conversational Architecture: Engineered an interactive `while True` continuous processing engine to capture and aggregate dynamic inputs across continuous conversational iterations
* Data Layer Merging: Utilizes list modification operators (`.extend()`) to scale contextual tracking arrays on-the-fly, driving continuous backend processing without re-initializing user states
* Exception & Validation Controls: Configured nested conditional fallbacks to flag unmapped data streams, handle exit queries, and process empty strings safely

### Knowledge Base Data Engineering
* Data Format Structure: JavaScript Object Notation (JSON) dictionary containing multi-layer nested parameters
* Modularity Architecture: Engineered file-handling modules utilizing the `json.load()` and `json.dumps()` file-transport serialization layers to separate the knowledge dataset from the core application script
* Exception Handling Interceptions: Configured robust error isolation blocks to catch file exceptions, system failures, and formatting corruptions during memory operations

---

## Project Performance and Quantifiable Data Points

When preparing resume bullet points or project metrics, utilize the following structural details from this codebase:

### 1. Linguistic Processing and Rule Engineering
* Search Constraints Managed: Programmed a 2-tier filtering verification loop that verifies if a word matches known symptoms while systematically blocking duplicate array entries
* Computational Target Mapping: Routes matching operations to map 3 parallel output attributes per condition: string identity variables, exact item frequency metrics, and localized clinical response scripts

### 2. Codebase Engineering and Architecture
* Pipeline Verification Steps: Configured 4 primary execution layers within the core chatbot workflow: structural file serialization, tokenized symptom extraction, multi-layered frequency ranking, and continuous stateful loop parsing

---

## Project Execution Guide

### 1. Local Environment Deployment
Install the required natural language processing engines, core English language pipelines, and standard libraries:
```bash
pip install spacy
python -m spacy download en_core_web_sm
```

### 2. Script Execution
Run the primary script file inside your environment terminal to build the database and verify the tokenization loop:
```bash
python main.py
```
