# CricIntel

CricIntel is an IPL data analytics Personal Project built on 17 seasons and 280,000+ deliveries of ball-by-ball cricket data. It covers the full data science pipeline from raw data cleaning and feature engineering to unsupervised player and venue clustering, ML-based match winner prediction, and first innings score prediction using powerplay and middle-over data as early indicators via Linear Regression. A custom NLP query engine sits on top of the entire system, routing natural language questions to the right analysis and returning ranked, visualised results. Whether you are a cricket fan, a data science learner, or a recruiter, CricIntel is designed to show what thoughtful, end-to-end data work looks like on a domain you are actually passionate about.

## Dataset
- File: `IPL.csv` from kaggle
- link: https://www.kaggle.com/datasets/chaitu20/ipl-dataset2008-2025
- Shape: 283,678 rows × 65 columns

## Methodology

| # | Stage | Description |
|---|-------|-------------|
| 1 | Data Collection & Loading | IPL ball-by-ball dataset spanning 17 seasons (2008–2024) with 280,000+ deliveries across 65 feature columns |
| 2 | Data Cleaning & Preprocessing | Standardised team and venue names, handled missing values, and engineered over phase, innings, and wicket features |
| 3 | Exploratory Data Analysis | Analysed team win rates, toss impact, venue scoring patterns, and built full batter, bowler, and head-to-head profiles |
| 4 | Venue Clustering — K-Means (K=3) | Clustered venues into Batting Paradise, Chaser Friendly, and Bowler Friendly archetypes based on scoring and chase patterns |
| 5 | Player Clustering — K-Means (K=4) | Grouped qualified batters into Explosive Hitter, Elite Anchor, Steady Accumulator, and Tailender archetypes based on batting style metrics |
| 6 | Match Winner Prediction — Random Forest | Trained a classifier on 12 engineered match-level features to predict the winning team before the match begins |
| 7 | Score Prediction — Linear Regression | Estimated final first innings score from powerplay and middle-over data using a regression model |
| 8 | NLP Query Engine | Built a rule-based query system from scratch that detects intent, extracts entities, and returns ranked visualised results for 10+ query types |

## Features
- Team performance analysis *(Pandas aggregations, comparative statistics, Matplotlib visualizations)*
- Toss impact analysis *(descriptive analysis, match outcome comparison)*
- Venue analysis *(venue-wise aggregation, trend analysis, visualization)*
- Batter and bowler statistics *(player-level feature engineering, strike rate/economy analysis)*
- Head-to-head comparisons *(player-vs-player and team-vs-team matchup analysis)*
- Player and venue pattern discovery *(K-Means clustering)*
- Match winner prediction *(Random Forest Classifier)*
- Final score prediction *(Linear Regression)*
- Query-based insights *(rule-based NLP using keyword matching and regex)*

## Techniques Used
- Exploratory Data Analysis (EDA)
- Data Cleaning and Preprocessing
- Feature Engineering
- K-Means Clustering
- Random Forest Classification
- Linear Regression
- Data Visualization
-Custom NLP query engine (regex + rule-based)
- Model Evaluation *(Accuracy Score, Classification Report, MAE, R² Score)*

## Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook / Google Colab



## Visualisation Outputs

This includes team win analysis, toss impact, venue clustering, batter/bowler analysis, player clustering, match prediction feature importance, NLP Query examples and score predictor outputs.


team win analysis:
<img width="1589" height="592" alt="team_win_analysis" src="https://github.com/user-attachments/assets/76daa00d-6ca4-4819-bf1c-878ed122bf01" />

venue clustering:
<img width="1775" height="1279" alt="K_means for type of venue" src="https://github.com/user-attachments/assets/4787a63f-1b0e-45ea-9d6b-e2fa18241bc7" />

<img width="1390" height="1180" alt="venue_stats" src="https://github.com/user-attachments/assets/d1742d19-5c9e-4d49-948b-9cc942075ed1" />

 batter/bowler analysis:
<img width="1785" height="1181" alt="bowler_analysis" src="https://github.com/user-attachments/assets/1a46ee19-ce35-4dd8-8fff-7439178587ae" />

<img width="1784" height="1180" alt="batter_analysis" src="https://github.com/user-attachments/assets/b46d89df-7af8-4f22-b052-11560755a4ba" />

player clustering:

<img width="1790" height="789" alt="K_means for type of batter" src="https://github.com/user-attachments/assets/eb555f8a-d4a2-4765-b2d4-e9c1b71e8151" />

match prediction feature importance:

<img width="1389" height="490" alt="featues for random forest match winner prediction" src="https://github.com/user-attachments/assets/c97cc3fe-0b25-4470-9b08-ce554f1186eb" />

<img width="889" height="290" alt="random forest_ match winner predictor" src="https://github.com/user-attachments/assets/39fe8c71-2130-4fc2-80a7-8398db037456" />

NLP Query examples:

<img width="395" height="256" alt="H2H matchup" src="https://github.com/user-attachments/assets/adc76e32-ae66-4337-af91-11b3a3f5e645" />

<img width="1289" height="490" alt="NLP ex 1" src="https://github.com/user-attachments/assets/d80fa3f9-8924-436a-9de8-cdfc9d82c9f1" />

<img width="1590" height="985" alt="nlp ex 3" src="https://github.com/user-attachments/assets/f306c7da-67f4-4bdb-99e7-25b20756c2ea" />

<img width="1289" height="490" alt="nlp example 4" src="https://github.com/user-attachments/assets/204bdd05-8307-430a-a474-80737eab554a" />

<img width="1623" height="495" alt="player comparison" src="https://github.com/user-attachments/assets/36c0e22e-ab71-490c-ad25-094b421fcd24" />

<img width="1289" height="489" alt="download" src="https://github.com/user-attachments/assets/93594cc8-c1a8-401a-a282-86e53463cec1" />





score predictor:

<img width="1389" height="495" alt="linear regression model for score predictor" src="https://github.com/user-attachments/assets/97922c23-d26f-4923-a15a-26cdb9c26a83" />

<img width="888" height="413" alt="Score prediction" src="https://github.com/user-attachments/assets/e5aa5452-09ac-4a48-bab2-c2f4d7530fbf" />







