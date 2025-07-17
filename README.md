# Computational analysis of Gender Perception in the UK Parliament 


This project investigates the changing importance of female-related terms in British parliamentary debates, with a particular focus on the period surrounding women’s suffrage in 1928. Developed entirely in Google Colab Pro, the codebase is optimized to minimize computational resource usage, especially for Retrieval-Augmented Generation (RAG) and Large Language Model (LLM) components. The analysis includes exploratory data analysis (EDA) of gendered pronoun counts, word clouds showing words co-occurring with target terms in selected years, and token-level plots tracking the prominence of specific words over time. To provide deeper context beyond EDA, a lightweight LLM-based system enables users to query the debates for information and sentiment related to suffrage and associated topics in documents from any chosen year or range of years. This approach ensures both efficiency and depth, allowing for nuanced exploration of gendered language trends in parliamentary history.

## Hypothesis
- 


## Data

- **Source:** [TheyWorkForYou.com](https://www.theyworkforyou.com/)
- **Download:** See `data/README.md` for instructions.

## Project Structure

- `notebooks/` — Jupyter notebooks for analysis
- `data/` — Data files extraction (not included in repo)
- `requirements.txt` — Python dependencies

## Results

This multi-method analysis of British parliamentary debates around the 1928 Equal Franchise Act reveals a consistent gender imbalance in both **pronoun usage** and **role framing**. While **female pronouns and TF-IDF importance spiked in 1928–1929**, these gains were not uniformly sustained in later years. **Word cloud results** show that women continued to be associated with **supporting or domestic roles**, while men were linked to **institutional power** and **political authority**.

RAG-based QA using a **small model on 1928 debates** surfaced both **supportive and oppositional arguments** on women's suffrage. The system effectively highlighted tensions between **moral duty**, **strategic concerns**, and **persistent stereotypes** around women’s political participation. While the results were insightful, future work with **larger models** and a **broader year range** could provide deeper understanding and richer historical context.

Refer to the [Results.ipynb](https://github.com/pk2971/computational-gender-analysis/blob/main/notebooks/Results.ipynb) notebook for more detailed evaluation of the results.


## Acknowledgments

- [TheyWorkForYou.com](https://www.theyworkforyou.com/) for data
- [spaCy](https://spacy.io/), [NLTK](https://www.nltk.org/), [LangChain](https://www.langchain.com/) for NLP tools


