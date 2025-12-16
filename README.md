[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/ritikade2/Social_Listening/blob/main/Social_Listening.ipynb
)

# Social Listening Projects

This repository contains **two independent social listening notebooks**, each demonstrating a different approach to analyzing social media conversations using Python.  
Both notebooks are intended for **exploratory analysis, research, and learning**, and are best run in **Google Colab**.

---

## Notebook 1: Rare Beauty Social Listening

**File:** `RareBeauty_Social_Listening.ipynb`

### Overview
This notebook focuses on **brand-specific social listening**, using *Rare Beauty* as a case study.  
It collects and analyzes public social media conversations (primarily Reddit) to explore user sentiment, recurring themes, and discussion patterns around the brand.

### What this notebook does
- Connects to Reddit using the official Reddit API (`praw`)
- Collects posts and comments from selected subreddits
- Filters comments using keyword-based logic
- Performs basic text preprocessing
- Applies sentiment analysis (VADER)
- Outputs structured results for qualitative review

### Data
- **Source:** Public Reddit posts and comments
- **PII:** No private or personal data is collected
- **Access:** Read-only API usage

### How to run
Open in Google Colab:

https://colab.research.google.com/github/ritikade2/Social_Listening/blob/main/RareBeauty_Social_Listening.ipynb

#### Requirements
You will need Reddit API credentials added as **Colab Secrets**:
- `REDDIT_CLIENT_ID`
- `REDDIT_CLIENT_SECRET`
- `REDDIT_USER_AGENT`

---

## Notebook 2: Social Analysis (File-Based)

**File:** `social_analysis.ipynb`

### Overview
This notebook provides a **general social text analysis pipeline** that works on an uploaded dataset rather than live API data.  
It is useful for analyzing comments, reviews, or posts collected from any social platform.

### What this notebook does
- Prompts the user to upload a dataset in Colab
- Cleans and preprocesses text data
- Performs sentiment analysis using VADER
- Extracts keywords and basic text statistics
- Produces summary outputs and visualizations

### Data
- **Source:** User-uploaded file (CSV or text-based)
- **Flexibility:** Can be reused for multiple platforms or datasets

### How to run
Open in Google Colab:

https://colab.research.google.com/github/ritikade2/Social_Listening/blob/main/social_analysis.ipynb

Steps:
1. Open the notebook in Colab
2. Upload the requested file when prompted
3. Run all cells
4. Review sentiment scores and summaries

---

## Repository Structure

```text
Social_Listening/
│
├── RareBeauty_Social_Listening.ipynb
├── social_analysis.ipynb
└── README.md
```


---

## Notes & Limitations

- These notebooks use **keyword-based filtering** and **lexicon-based sentiment analysis**
- Results depend heavily on data quality and platform activity
- This is not a production-grade scraping system
- Reddit API rate limits and terms of service apply

---

## Disclaimer

This project is intended for **educational and research purposes only**.  
All data used is publicly available, and no attempt is made to identify or profile individuals.

