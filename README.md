# AI Study Engine

Generate Flashcards, Quizzes, and Summaries from any text using AI.

---

## Features

- **Flashcards:** Generate multiple question-answer pairs from study text.
- **Quizzes:** Create MCQs with 4 options and the correct answer marked.
- **Summary:** Summarize long notes into concise bullet points.

---

## Project Structure

ai-study-engine/
│
├── main.py
├── .env
├── config/
│ └── settings.py
├── providers/
│ ├── groq_provider.py
├── prompts/
│ ├── flashcard_prompt.py
│ ├── quiz_prompt.py
│ └── summary_prompt.py
├── services/
│ ├── flashcard_service.py
│ ├── quiz_service.py
│ └── summary_service.py
├── ui/
│ └── app.py
├── requirements.txt
├── .gitignore
└── README.md


---

## Setup Instructions

1. Clone this repository:
```bash
git clone <YOUR_REPO_LINK>
cd ai-study-engine

2. Create virtual environment:

python -m venv venv
```bash
# Activate venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

3. Install dependencies:
```bash
pip install -r requirements.txt

4. Add environment variable:

Copy .env.example → .env

Paste your Groq API Key:
ini
GROQ_API_KEY=your_real_groq_api_key


How to Run Locally
Run Streamlit UI:
```bash
streamlit run ui/app.py

Example Input/Output
Input Text:
Machine learning is a field of artificial intelligence.
It allows systems to learn from data.
Supervised learning uses labeled data.
Unsupervised learning works with unlabeled data.

Flashcards Output (JSON):
{
  "flashcards": [
    {"question": "What is machine learning?", "answer": "A field of AI where systems learn from data."},
    {"question": "What does supervised learning use?", "answer": "Labeled data."}
  ]
}





