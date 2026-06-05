# amazon-prime-tv-movies---shows-analysis
data analytics project showcasing amazon prime tv movies and shows analysis using python, pandas, NumPy and tableau.
📺 Amazon Prime TV Shows & Movies Analysis
📌 Project Overview

This project performs an end-to-end Exploratory Data Analysis (EDA) on the Amazon Prime Movies and TV Shows dataset using Python and Tableau. The objective is to uncover content trends, audience preferences, genre distribution, regional content patterns, ratings behavior, and release trends that can support content strategy and business decision-making.

🎯 Business Problem

Streaming platforms continuously expand their content libraries. Understanding what type of content performs well, how content is distributed across genres and regions, and how audience ratings relate to content characteristics is essential for improving content acquisition and production strategies.

This project aims to answer questions such as:

Which genres dominate Amazon Prime's catalog?
Which regions contribute the most content?
Has content production increased over time?
Do longer titles receive better ratings?
How does content popularity relate to audience ratings?
What proportion of content is recent versus older content?
📂 Dataset Information

Dataset Source: Amazon Prime Movies & TV Shows Dataset

Files Used
titles.csv
credits.csv
Dataset Size After Cleaning
Dataset	Records
Titles	9,868
Credits	124,179
Final Merged Dataset	9,868
🛠️ Tools & Technologies
Python
Pandas
NumPy
Matplotlib
Seaborn
Ast
Visualization
Tableau Public
Development Environment
Google Colab
GitHub
🧹 Data Cleaning & Preprocessing
Duplicate Handling
Removed duplicate records from both datasets.
Missing Value Treatment
Filled missing age certifications with "Not Rated".
Replaced missing season values with 0.
Imputed missing IMDb and TMDB metrics using median values.
Removed records with missing titles.
Replaced missing character information with "No Character Info".
Data Type Corrections

Converted all analytical columns into appropriate numeric formats.

⚙️ Feature Engineering

Created several new business-focused features:

Feature	Description
Content Age	Years since release
Decade	Release decade
Runtime Category	Short, Medium, Long, Very Long
Rating Category	Bad, Good, Very Good, Excellent
Popularity Category	Low to Very High Popularity
IMDb Vote Category	Voting engagement level
Genre Category	Consolidated genre groups
Country Region	Regional classification
Number of Genres	Count of assigned genres
Is Recent	Content released after 2018
🔗 Data Integration

The Credits dataset contains multiple cast and crew members per title.

To prevent duplicate records after merging:

Aggregated cast names
Aggregated roles
Aggregated characters

Merged the cleaned Titles and Credits datasets using the unique content ID.

Result:

✅ One row = One title

📊 Tableau Dashboard
Key KPIs
Total Titles
Total Movies
Total TV Shows
Average IMDb Score
Average TMDB Popularity
Visualizations
1. Genre Distribution

Displays content distribution across major genre categories.

Insight:
Entertainment and Emotional content dominate the platform.

2. Regional Content Distribution (Map)

Visualizes content production across geographic regions.

Insight:
North America contributes the largest share of content.

3. Runtime vs IMDb Score

Analyzes the relationship between content duration and audience ratings.

Insight:
Medium and long-form content generally receive stronger ratings.

4. Rating Category by Genre

Compares content quality across genre categories.

Insight:
Drama-heavy categories contain a larger share of highly-rated titles.

5. Release Trend Analysis (Dual Axis)

Tracks content releases over time.

Insight:
Content production accelerated significantly after 2010.

6. Recent vs Old Content

Compares modern and legacy content.

Insight:
Recent content forms a major portion of the catalog, reflecting Amazon Prime's focus on fresh content.

📈 Key Business Insights
Content Strategy
Emotional and entertainment-focused genres dominate audience demand.
Recent content additions drive platform growth.
Regional Expansion
North America remains the largest content-producing region.
Opportunities exist to expand content acquisition in Asia and Europe.
Quality Analysis
Higher-rated content is concentrated in specific genre categories.
Runtime length shows a moderate relationship with audience ratings.
Content Investment
Consistent growth in releases suggests aggressive content expansion.
Historical content remains valuable for maintaining catalog depth.
📋 Project Workflow
Data Loading
Data Understanding
Duplicate Removal
Missing Value Treatment
Data Type Conversion
Feature Engineering
Dataset Integration
Exploratory Data Analysis
Tableau Dashboard Development
Business Insight Generation
📸 Dashboard Preview

Add dashboard screenshots inside the /Images folder and embed them here.

Example:

![Dashboard](Images/dashboard.png)
🚀 Future Enhancements
Build predictive models for IMDb ratings.
Create recommendation systems based on genres.
Perform sentiment analysis using content descriptions.
Develop an interactive web dashboard using Streamlit or Power BI.
👨‍💻 Author

Rudraneel Dutta

Aspiring Data Analyst | Python | SQL | Tableau | Power BI

GitHub: https://github.com/rudraneeldutta33-glitch

⭐ Project Outcome

Successfully transformed raw Amazon Prime content data into an analysis-ready dataset, built an interactive Tableau dashboard, and generated actionable business insights regarding content distribution, ratings, genres, regional trends, and platform growth.
