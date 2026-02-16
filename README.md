# Civic Discourse to Policy

A Streamlit web application that analyzes local Reddit discourse to identify the most discussed civic issues in a community and generates AI-assisted policy platform recommendations.

Built as an independent project to explore how natural language processing can bridge the gap between public discourse and actionable policy, helping policymakers understand what communities actually care about.

**[Live App](https://pittsburghcampaigncrystallizer.streamlit.app/)**

## What It Does

The app scrapes and analyzes posts from local subreddits (e.g., r/pittsburgh) to:

1. **Identify top civic issues** — categorizes 1,000+ posts into issue areas like housing, transportation, safety, and government services
2. **Visualize community priorities** — generates bar charts and word clouds showing what residents discuss most
3. **Generate policy recommendations** — uses OpenAI's API to produce policy platform planks grounded in real community concerns
4. **Enable drill-down analysis** — lets users explore individual posts within each issue category

## Tech Stack

Python, Streamlit, Pandas, Plotly, WordCloud, OpenAI API

## Project Structure

```
├── data/
│   ├── cleaned_posts.csv
│   └── platform_planks.csv
├── scripts/
│   ├── clean_and_label.py
│   ├── platform_plank_generator.py
│   └── visualise.py
├── .streamlit/
│   └── secrets.toml (excluded from Git)
├── requirements.txt
└── README.md
```

## Run Locally

```bash
git clone https://github.com/ks0046/Civic-Discourse-to-Policy.git
cd Civic-Discourse-to-Policy
pip install -r requirements.txt
```

Create `.streamlit/secrets.toml` and add your OpenAI API key:

```
OPENAI_API_KEY = "your-api-key-here"
```

Launch:

```bash
streamlit run scripts/visualise.py
```

## Author

**Kriti Samnotra**
MS Public Policy & Management (DC Track), Carnegie Mellon University
[LinkedIn](https://www.linkedin.com/in/kriti-samnotra/)
