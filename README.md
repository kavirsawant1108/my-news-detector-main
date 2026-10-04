# Fake News Detection System

> NLP-based fake news classification system using machine learning, React, TypeScript, and Supabase.

## Overview

The Fake News Detection System explores how Natural Language Processing (NLP) and machine learning can be used to classify news articles.

The project demonstrates an end-to-end workflow: text preprocessing, feature extraction, model training, evaluation, prediction, and a web interface for interacting with the classifier.

## Key Features

- Real vs. fake news classification
- Text preprocessing for news content
- Machine-learning based prediction
- Interactive React web interface
- Supabase integration where configured
- Production build workflow through Vite

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React, TypeScript, Vite |
| UI | Tailwind CSS |
| Machine Learning | Python, Scikit-learn, NLTK |
| Data / Backend Services | Supabase |
| Tooling | Node.js, npm |
| Version Control | Git / GitHub |

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
- Python environment for the ML components
- A configured Supabase project if Supabase-backed features are used

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

For a production-quality ML report, publish measured results for:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

Performance numbers should only be added after evaluation on a defined test set.

## Security

- Environment-specific configuration belongs in `.env`.
- Only non-sensitive placeholders belong in `.env.example`.
- Review Supabase Row Level Security policies before deployment.
- Never commit service-role keys, database passwords, or other privileged credentials.

## Limitations

- Classification quality depends heavily on dataset quality and distribution.
- A model trained on historical news may not generalize to new sources or writing styles.
- A model prediction is not a substitute for professional fact-checking.

## Future Improvements

- Add reproducible training scripts
- Publish evaluation results and confusion matrix
- Add automated tests
- Improve model monitoring
- Add CI checks
- Containerize the application
- Deploy a production demo

## License

Add a license when project ownership and reuse terms are confirmed.
