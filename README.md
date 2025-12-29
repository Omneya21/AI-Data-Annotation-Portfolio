# AI Data Annotation Portfolio: NLP, Sentiment & LLM Workflows

## 📌 Project Overview
This repository demonstrates a professional workflow for high-quality data annotation and dataset preparation, specifically designed for training Machine Learning and Large Language Models (LLMs). Using the **IMDb Movie Reviews dataset**, I showcase the end-to-end process from raw text cleaning to advanced entity extraction and quality assurance.

## 🎯 Key Skills Demonstrated
* **Named Entity Recognition (NER):** Extracting key entities (Actors, Titles, Organizations) using spaCy.
* **Sentiment Annotation:** Classifying text sentiment and identifying patterns.
* **Quality Assurance (QA):** Flagging low-quality, ambiguous, or outlier data for manual review.
* **LLM-Assisted Annotation:** Prompt engineering for automated labeling and cross-validation with human-in-the-loop workflows.
* **Data Cleaning:** Removing HTML noise and preprocessing text for model readiness.

## 🛠 Tech Stack
* **Python** (Pandas, Numpy)
* **NLP:** spaCy, BeautifulSoup
* **Visualizations:** Matplotlib, Displacy
* **AI Tools:** Prompt Engineering for LLMs (GPT/Claude/Gemini)

## 📑 Annotation Workflow & Guidelines

### 1. Data Cleaning & Preprocessing
Raw reviews often contain HTML tags and noise. I implemented a cleaning pipeline to ensure text integrity before the annotation phase.

### 2. Entity Extraction (NER)
I defined specific rules for identifying entities:
- **WORK_OF_ART:** Movie titles, series, and books.
- **PERSON:** Actors, directors, and crew members.
- **ORG:** Production companies and studios.

### 3. Quality Control (The "Annotator" Mindset)
A crucial part of this project is identifying **ambiguous data**. 
- **Flagging:** Reviews with fewer than 5 entities are flagged as "low-context" for manual verification.
- **Validation:** High-priority samples (reviews mentioning specific titles) are isolated for a second pass of human validation.

### 4. LLM Integration (Prompt Engineering)
I developed a **Prompt Engineering** framework to use LLMs as "Co-Annotators". This includes:
- Multi-step prompts to extract structured JSON data.
- Comparison between traditional NLP (spaCy) and LLM-based extraction to ensure the highest accuracy.

## 🔊 Audio & Voice Annotation Expertise (Methodology)
*While this notebook focuses on text, my workflow for audio data includes:*
- **Speaker Diarization:** Labeling multiple speakers in a conversation.
- **Non-Speech Events:** Tagging background noise, laughter, and pauses.
- **Verbatim vs. Clean Transcription:** Handling filler words (uh, um) based on project requirements.
- **Quality Scoring:** Evaluating audio clarity and transcription accuracy.

## 📊 Insights & Visualizations
The project includes automated reports on:
- Entity frequency distribution.
- Sentiment skewness in title-heavy reviews.
- Mean entity count per record for dataset balancing.
