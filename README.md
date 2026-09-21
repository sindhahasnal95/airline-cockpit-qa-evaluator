# airline-cockpit-qa-evaluator
GenAI-powered Airline Cockpit Voice Recorder and ATC-Pilot communication QA evaluation using LangChain.

Airline Cockpit Voice Recorder / ATC-Pilot QA Evaluator

Project Overview

The Airline Cockpit Voice Recorder / ATC-Pilot QA Evaluator is a GenAI-powered application designed to evaluate ATC-Pilot communication transcripts using Large Language Models (LLMs) and LangChain.

The application classifies transcripts, dynamically routes them to relevant QA criteria, evaluates communication quality, and generates a final QA report with actionable recommendations.

This project was developed as a capstone project as part of my Generative AI learning journey.

Objectives
Classify ATC-Pilot communication transcripts.
Route transcripts to relevant QA evaluation criteria.
Evaluate communication using an LLM-based evaluation chain.
Generate scores, reasoning, and transcript-based evidence.
Produce a professional summary and actionable recommendations.
Demonstrate LangChain orchestration and structured LLM outputs.

Architecture
Transcript CSV
     |
     v
LLM Classification
     |
     v
Rule-Based Routing
     |
     v
Evaluation Plan
     |
     v
Airline QA Evaluation Chain
     |
     v
Score Aggregation
     |
     v
Final Report Generation
     |
     v
QA Summary and Recommendations

QA Evaluation Criteria
Readback / Hearback Accuracy
Phraseology Compliance
CRM Coordination
Situational Awareness

Classification Categories
routine_operations
minor_abnormal_event
critical_emergency
weather_deviation

Technology Stack
Python
LangChain
Pydantic
Pandas
OpenAI or Gemini LLM
Jupyter Notebook / PyCharm
Git and GitHub

Key Features
Transcript classification using an LLM.
Structured output parsing using Pydantic.
Configuration-driven evaluation criteria.
Dynamic criterion-based QA evaluation.
Score and reasoning generation.
Final summary and recommendations.
Batch processing of transcripts.


Getting Started:
1. Clone the repository
git clone https://github.com/YOUR_USERNAME/airline-cockpit-qa-evaluator.git
cd airline-cockpit-qa-evaluator
2. Create a virtual environment
python -m venv .venv
3. Activate the environment on Windows
.venv\Scripts\activate
4. Install dependencies
python -m pip install -r requirements.txt
5. Configure environment variables

Create a local .env file and configure your LLM provider credentials.

Do not commit API keys or sensitive credentials to the repository.

6. Run the application

Follow the execution instructions provided in the project source code or notebook.

Evaluation Output

The application produces:

Predicted call type
Classification confidence
Criterion-level QA scores
Reasoning and evidence
Overall evaluation summary
Actionable recommendations

Project Structure
airline-cockpit-qa-evaluator/
├── data/
├── notebooks/
├── src/
├── config.json
├── requirements.txt
├── README.md
└── .gitignore

Future Enhancements
Add a Streamlit dashboard.
Support audio-to-text transcription.
Add human reviewer feedback.
Add evaluation score visualizations.
Add automated test cases for prompt and classification quality.
Add experiment tracking and model comparison.

Author
Sindha Hasnal Kareem

Disclaimer

This project is an educational GenAI capstone project. It is not intended for operational aviation safety decisions, flight control, or regulatory certification.
