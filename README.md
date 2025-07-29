# Building-a-Text-Classification-Pipeline-Word-Embedding-Exploration
 design an end‑to‑end Natural Language Processing (NLP) pipeline that turns raw text into actionable insights.

## Project Tasks & Milestones

### 1. Data Acquisition & Exploration 

- Download & inspect the raw corpus; summarise size, classes, class balance.
- Show 3–5 representative examples per class.

### 2. Pre‑processing Pipeline 

- Implement a clean, reusable pipeline that performs **lower‑casing, regex cleaning, tokenisation, stop‑word removal, and stemming *or* lemmatisation**.
- Demonstrate the impact on at least one example string.

### 3. Feature Engineering 

- **Sparse**: Build both **Bag‑of‑Words** and **TF‑IDF** feature matrices (uni‑gram + optional bi‑gram).
- **Dense**: Train **Word2Vec (CBOW or Skip‑Gram)** on the training split *or* use a pre‑trained embedding (e.g. `gensim‑downloader`) and average the token vectors to obtain document‑level embeddings.
- (Optional ⭐) Train a simple **character 3‑gram Markov chain** and generate 5 sample sentences.

### Modelling & Evaluation (30 pts)

- Split data into train/validation/test (suggested 70/10/20).
- Train **Multinomial Naïve Bayes** on the sparse representations.
- Train **Logistic Regression *or* Linear SVM** on both sparse and dense representations.
- Evaluate using **accuracy + precision, recall, F1‑score** (macro‑average if classes > 2).
- Present results in a concise table.

### 5. Analysis & Discussion (10 pts)

- Compare generative vs. discriminative performance.
- Discuss how N‑gram size and embedding choice affected results.
- Reflect on speed, memory, and explainability.

### 6. Reproducibility & Code Quality (10 pts)

- All code must be **well‑commented** and organised in a single Jupyter notebook **or** Python script package with clear function boundaries.
- Use **`requirements.txt`** / environment yaml.
- Seed all random operations.

   
