# A2SV Eskalate NLP Task

This project implements the A2SV Eskalate NLP interview task, covering:

1. **Data Preparation & Exploration**
2. **Information Extraction & Summarization**
3. **Agentic System Design (News Aggregator Agent)**

## Dataset
- **Kaggle News Category Dataset** (~210k news articles, 2012–2022)
- Download from: https://www.kaggle.com/datasets/rmisra/news-category-dataset
- Place `News_Category_Dataset_v3.json` in the project directory.

## Environment
- Recommended: Google Colab or local Jupyter with GPU for T5 summarization
- Requires Python 3.8+

## Setup Instructions
1. **Install dependencies**
   - Run the following in a notebook cell or terminal:
     ```
     pip install -r requirements.txt
     python -m spacy download en_core_web_sm
     ```
2. **Run the Notebook**
   - Open `a2sv_nlp_task.ipynb` in Jupyter or Colab.
   - Execute cells sequentially.
   - Ensure a GPU is available for efficient summarization.

## Features
- **Data Preparation**: Cleans and tokenizes news headlines and descriptions.
- **Exploration**: Visualizes word and entity distributions.
- **Information Extraction**: Extracts dates, metrics, and named entities.
- **Summarization**: Provides both extractive (TextRank) and abstractive (T5) summaries.
- **Agentic System**: A working News Aggregator Agent answers user queries using the dataset.

## Extensibility
- Swap T5 for Gemma or other models as needed.
- Enhance query parsing with BERT or similar models.

## Notes
- For large datasets, consider chunked loading and parallel processing.
- T5 summarization is slow without a GPU.

## License
This project is for educational and interview purposes only.
