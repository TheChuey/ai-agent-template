The purpose of the file is to create a template for starting projects. It contains starter code to set up the environment where the code will live. These are notes for those who need a refresher and a quicker way to start coding.

---

# PROJECT SETUP GUIDE

---

*** STEP 1 — CREATE requirements.txt ***

---

Create a file named `requirements.txt` and add:

langchain
langchain-openai
langchain-anthropic
pydantic
python-dotenv
wikipedia
duckduckgo-search

---

*** STEP 2 — CREATE VIRTUAL ENVIRONMENT (Recommended) ***

---

This creates an isolated environment for your project dependencies.

Windows:
python -m venv venv

Mac / Linux:
python3 -m venv venv

---

*** STEP 3 — ACTIVATE VIRTUAL ENVIRONMENT ***

---

Windows:
.\venv\Scripts\activate

Mac / Linux:
source venv/bin/activate

When activated, your terminal will show:
(venv)

---

*** STEP 4 — INSTALL DEPENDENCIES ***

---

pip install -r requirements.txt

---

*** STEP 5 — PROJECT FILE STRUCTURE ***

---

project-root/
│
├── main.py        # Primary application logic
├── tools.py       # Tool definitions
├── requirements.txt
└── .env           # Environment variables (DO NOT COMMIT)

---

*** STEP 6 — SET UP ENVIRONMENT VARIABLES ***

---

Create a `.env` file in the project root:

OPENAI_API_KEY=your_openai_key_here
ANTHROPIC_API_KEY=your_anthropic_key_here

Generate API keys from:

OpenAI: [https://platform.openai.com](https://platform.openai.com)
Anthropic: [https://console.anthropic.com](https://console.anthropic.com)

Never push your `.env` file to GitHub.
