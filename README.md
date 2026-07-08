# AI-Powered Medical Diagnosis Assistant Chatbot

An interactive text-based medical diagnosis assistant built in Python using **spaCy** for Natural Language Processing (NLP). The chatbot analyzes user symptoms, matches them against a pre-defined JSON knowledge base, calculates the likelihood of conditions based on overlapping symptoms, and provides preliminary wellness advice alongside standard medical disclaimers.

## Features

* **Natural Language Processing**: Uses `spaCy` to process unstructured conversational text inputs.
* **Smart Intent Recognition**: Safely handles lowercase matching and variations of symptom terms.
* **Weighted Condition Mapping**: Sorts potential medical diagnoses by likelihood according to matching symptom frequencies.
* **Multi-Turn Conversation**: Continually prompts the user for supplementary symptoms until they type "no", dynamically recalculating diagnoses.
* **Modular System Design**: Decoupled JSON data persistence layer makes it easy to integrate with web apps like Flask or Django later.

---

## 🛠️ Requirements & Setup

Make sure you have Python 3.8+ installed on your system. 

### 1. Install Dependencies
Install the required packages. To avoid workspace compatibility conflicts, this application works best with `spaCy` version `3.7.2`:
```bash
pip install spacy==3.7.2
```

### 2. Download the English NLP Model
The chatbot uses spaCy's small core English language model package to tokenize and structuralize conversational variables:
```bash
python -m spacy download en_core_web_sm
```

---

## How to Run the Code

1. Save the chatbot program on your computer as a file named `medical_chatbot.py`.
2. Run the application from your terminal or command prompt:
```bash
python medical_chatbot.py
```

---

## How to Use the Chatbot

1. **Initial Concern**: The chatbot will start and ask you: `Please enter your primary concern:`.
   * *Example input:* `"I have a bad headache and a terrible fever."`
2. **Dynamic Review**: The program matches your terms against the system's `medical_data.json` schema and reports the most likely conditions first.
3. **Multi-Turn Extension**: The system then prompts you for more symptoms: `Please enter an additional symptom, or 'no' if you have no more:`.
   * Add extra terms like `"fatigue"` or `"chills"` to see the match counter increase.
4. **Exit**: Type `no`, `nope`, or `none` to quit the loop and print your final health summary.

---

## Knowledge Base Architecture (`medical_data.json`)

The script automatically generates a local structured dictionary database containing mapping relations like:
* **Symptoms**: Linked to several target conditions (e.g., `cough` maps to *common cold*, *flu*, *bronchitis*, *pneumonia*, and *allergies*).
* **Recommendations**: Associated actionable support instructions for individual matches.

---

## Medical Disclaimer
This software application is a rule-based prototype developed for educational and experimental purposes. It does not provide medical advice. It cannot substitute for professional human medical evaluation, triage, diagnosis, or targeted clinical therapy. Always consult an authorized healthcare provider for actual medical concerns.
