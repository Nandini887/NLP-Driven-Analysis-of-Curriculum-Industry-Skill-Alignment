# NLP-Driven-Analysis-of-Curriculum-Industry-Skill-Alignment
This project analyzes whether top global MS in Business Analytics (MSBA) programs teach the same skills that employers demand in Data Analyst, Business Analyst, and Data Scientist roles. Using web-scraped curriculum descriptions and job postings, the project applies an end-to-end NLP pipeline—including text preprocessing, feature extraction, cosine similarity, and topic modeling—to quantify alignment and identify gaps in technical and analytical skill coverage.

# Project Overview

Universities advertise a wide range of analytics-related courses, but it is unclear how well these programs map to real industry needs. This project evaluates skill alignment by:

Collecting curriculum descriptions from top MSBA programs.

Scraping job postings from Indeed for analytics roles.

Preprocessing and vectorizing text to extract meaningful features.

Measuring similarity between curriculum skills and job-required skills.

Using LDA topic modeling to uncover hidden themes in job descriptions.

Visualizing gaps in analytics, ML, statistics, and cloud competencies.

The output helps identify which academic programs are aligned with industry expectations and where skill mismatches exist.

### Methods & Workflow
1. Data Collection

Curriculum descriptions scraped from global MSBA program websites

Job postings scraped from Indeed for:

Data Analyst

Business Analyst

Data Scientist

2. Text Preprocessing

Performed standard NLP cleaning:

Tokenization

Lowercasing

Stopword removal

Lemmatization

Regex cleaning

3. Feature Engineering

CountVectorizer for bag-of-words feature extraction

Cosine Similarity to evaluate curriculum ↔ job skill overlap

LDA Topic Modeling to discover high-level skill groups such as:

Machine Learning

SQL & Data Engineering

Statistics

Cloud Tools

Business Intelligence

4. Evaluation Framework

Each university program is evaluated on:

Skill Similarity Score (cosine similarity)

Topic Coverage (distribution of LDA topics)

Keyword Demand Gap (skills mentioned in jobs but missing in curriculum)

5. Visualization & Insights

Built visual outputs including:

Heatmaps showing similarity strength

Bar charts of topic importance

Word clouds for top skills

Comparative plots of universities vs. job skill needs

Key insights revealed:

A measurable curriculum–industry gap in ML, cloud platforms, and NLP

Stronger alignment with business analysis skills than with data science skills

Variation in technical rigor across universities

# Key Results

CountVectorizer + cosine similarity exposed low overlap for ML, cloud, and NLP skills in many programs.

LDA topic modeling showed job postings emphasize machine learning, SQL, statistics, and cloud, while some curriculums focus more on business foundations.

Highlighted actionable recommendations for aligning academic programs with employer expectations.

### Technologies Used

Languages & Libraries:

Python, Pandas, NumPy

Scikit-learn (CountVectorizer, LDA, cosine similarity)

NLTK (lemmatization, stopword removal)

Gensim (topic modeling)

Matplotlib, Seaborn

Tools:

Jupyter Notebook

GitHub
