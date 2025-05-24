# 📰 News Recommendation Analysis

## 📌 Overview
This project analyzes user behavior and news article data to explore **category diversity** in user interactions over time. The core notebook (`k.ipynb`) processes the datasets, visualizes news category distributions, and tracks the **average number of unique categories** users engage with on a daily basis.

---

## 🎯 Purpose

The primary objectives of this project are:

- **Data Loading and Preprocessing**  
  Load and preprocess data from TSV files containing news and user behavior information.

- **Exploratory Data Analysis (EDA)**  
  Visualize the distribution of news categories to understand dataset composition.

- **Temporal Analysis**  
  Track how the diversity of news categories (unique categories clicked per user) changes over time.

---

## 📂 Dataset

This analysis uses two tab-separated value (TSV) files:

### `news.tsv`
Contains news article details:
- `news_id`: Unique article identifier  
- `category`: Broad category (e.g., lifestyle, news, health)  
- `subcategory`: Specific subcategory (e.g., lifestyleroyals, newsworld)  
- `title`: Article title  
- `abstract`: Brief summary (may contain `NaN` values)  
- `url`: Article URL  
- `title_entities`: Entities from title  
- `abstract_entities`: Entities from abstract  

### `behaviors.tsv`
Contains user interaction data:
- `impression_id`: Unique identifier for the impression  
- `user_id`: Unique user identifier  
- `timestamp`: Date and time of interaction  
- `user_history`: Space-separated list of news IDs user interacted with  
- `impressions`: List of shown news IDs with click indicators (e.g., `N12345-1` for clicked)

> **Requirement**: Ensure both files are placed in the same directory as `k.ipynb`.

---

## 🧩 Dependencies

Install required Python libraries:

```bash
pip install pandas matplotlib seaborn
