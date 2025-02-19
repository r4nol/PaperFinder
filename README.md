# PaperFinder

## Overview
A scientific article recommendation system that leverages Sentence Transformers and cosine similarity to suggest relevant articles based on user queries. This project processes an arXiv dataset, encodes article summaries into embeddings, and finds the most similar articles to the user’s search query.

## Features
- Uses a **SentenceTransformer** model (`paraphrase-multilingual-MiniLM-L12-v2`) for text embeddings.
- Calculates **cosine similarity** to match user queries with relevant scientific articles.
- Displays search results in a **rich-text table** for better readability.
- Supports **GPU acceleration** for fast inference using PyTorch.

## Installation

### Prerequisites
Ensure you have the required dependencies installed:

Install dependencies from `requirements.txt`:
```bash
pip install -r requirements.txt
```

## Usage

### 1. Prepare Dataset
Place the `arXiv_scientific dataset.csv` file in the root directory.

### 2. Open the Jupyter Notebook
Launch Jupyter Notebook and open `PaperFinder.ipynb`:
```bash
jupyter notebook PaperFinder.ipynb
```

### 3. Run the Notebook
- Execute the cells step by step.
- When prompted, enter a query in the input field.
- The system will return the top 5 most relevant articles with match percentages.

### 4. Example Query
After running the notebook, input a query such as:
```bash
Enter query (or 'exit' to stop): We propose an improved dependency-directed backtracking method that reduces search progress loss by moving backtracking points deeper into space while preserving polynomial memory and completeness guarantees.
```
It will return the top 5 most relevant articles along with match percentages.

## Repository Structure
```
├── arXiv_scientific dataset.csv  # Dataset file
├── PaperFinder.ipynb             # Jupyter Notebook version
├── requirements.txt              # Dependencies file
├── README.md                     # Documentation
```

## License
This project is licensed under the MIT License.
