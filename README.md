# Computational analysis of Gender Perception in the UK Parliament 


This project investigates the changing importance of female-related terms in British parliamentary debates, with a particular focus on the period surrounding women’s suffrage in 1928. Developed entirely in Google Colab Pro, the codebase is optimized to minimize computational resource usage, especially for Retrieval-Augmented Generation (RAG) and Large Language Model (LLM) components. The analysis includes exploratory data analysis (EDA) of gendered pronoun counts, word clouds showing words co-occurring with target terms in selected years, and token-level plots tracking the prominence of specific words over time. To provide deeper context beyond EDA, a lightweight LLM-based system enables users to query the debates for information and sentiment related to suffrage and associated topics in documents from any chosen year or range of years. This approach ensures both efficiency and depth, allowing for nuanced exploration of gendered language trends in parliamentary history.


## Data

- **Source:** [TheyWorkForYou.com](https://www.theyworkforyou.com/)
- **Download:** See `data/README.md` for instructions.

## Project Structure

- `notebooks/` — Jupyter notebooks for analysis
- `src/` — Source code
- `data/` — Data files (not included in repo)
- `requirements.txt` — Python dependencies


## Acknowledgments

- [TheyWorkForYou.com](https://www.theyworkforyou.com/) for data
- [spaCy](https://spacy.io/), [NLTK](https://www.nltk.org/), [LangChain](https://www.langchain.com/) for NLP tools


