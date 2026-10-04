# Fake News Detection System

> An NLP and machine-learning application that classifies news content as real or fake through text preprocessing and predictive modeling.

## Overview

The Fake News Detection System explores how Natural Language Processing (NLP) and machine learning can be used to classify news articles.

The project focuses on the complete ML workflow: preparing text, extracting useful features, training a classifier, evaluating results, and exposing predictions through a web interface.

## Features

- Real vs. fake news classification
- Text preprocessing for news content
- Machine-learning based prediction
- Interactive web interface
- Supabase integration for application data where configured

## Tech Stack

- **Frontend:** React, TypeScript, Vite
- **UI:** Tailwind CSS
- **Machine Learning:** Python, Scikit-learn, NLTK
- **Data / Backend Services:** Supabase
- **Application tooling:** Node.js, npm
- **Version Control:** Git / GitHub

> This README intentionally lists the technologies actually represented by the repository instead of alternatives such as “Flask / Django / Streamlit”.

## ML Pipeline

```text
News Dataset
     │
     ▼
Text Cleaning
     │
     ▼
Tokenization / Vectorization
     │
     ▼
Feature Extraction
     │
     ▼
Model Training
     │
     ▼
Evaluation
     │
     ▼
Prediction
     │
     ▼
Web Interface
```

## Getting Started

### Prerequisites

- Node.js
- npm
- A configured Supabase project if the application features requiring Supabase are used

### Installation

```bash
git clone https://github.com/kavirsawant1108/my-news-detector-main.git
cd my-news-detector-main
npm install
```

### Environment Variables

Create a local `.env` file based on `.env.example`.

Never commit the real `.env` file.

```env
VITE_SUPABASE_URL=
VITE_SUPABASE_PUBLISHABLE_KEY=
```

### Run Locally

```bash
npm run dev
```

### Production Build

```bash
npm run build
```

## Project Structure

```text
my-news-detector-main/
├── src/
├── public/
├── docs/
├── .env.example
├── .gitignore
├── package.json
└── README.md
```

## Model Evaluation

For a production-quality ML report, record and publish the measured:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Do not claim performance numbers unless they have been measured on a defined test set.

## Security

- Environment-specific configuration belongs in `.env`.
- Only non-sensitive placeholders belong in `.env.example`.
- Review Supabase Row Level Security policies before deployment.
- Never commit service-role keys, database passwords, or other privileged credentials.

## Limitations

- Classification quality depends heavily on dataset quality and distribution.
- A model trained on historical news may not generalize to new sources or writing styles.
- “Real” or “fake” classification should be treated as a model prediction, not a substitute for human fact-checking.

## Future Improvements

- Add reproducible training scripts
- Publish evaluation results and confusion matrix
- Add automated tests
- Improve model monitoring
- Add CI checks
- Containerize the application
- Deploy a production demo

## License

Add a license when the project's ownership and reuse terms are confirmed.
