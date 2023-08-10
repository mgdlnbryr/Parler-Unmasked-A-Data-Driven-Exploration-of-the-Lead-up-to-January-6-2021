# Parler Unmasked: A Data-Driven Exploration of the Lead-up to January 6, 2021
## Overview
This project aims to perform an in-depth analysis of text data collected from the Parler social media platform, particularly focusing on the months leading up to the January 6, 2021 insurrection. The analysis encompasses clustering, topic modeling, trend analysis, and visualization to uncover insights into the content and behavior of users on the platform.

## Data
The [dataset](https://github.com/sbooeshaghi/parlertrick) consists of user posts from Parler, including post content, timestamps, hashtags, and other relevant metadata. The data was cleaned and preprocessed for analysis.

## Methodology
### Clustering
**Vectorization:** Text data was transformed into numerical format using the CountVectorizer, extracting meaningful features and representing documents as a document-term matrix.

**Clustering Algorithm:** MiniBatchKMeans clustering was applied to partition the data into distinct groups, revealing common themes and patterns within the data. The optimal number of clusters was determined using the Elbow and Silhouette methods.
### Topic Modeling
**Latent Dirichlet Allocation (LDA):** LDA was employed to discover hidden topics in the text data, representing each topic as a distribution over words. The results were visualized using pyLDAvis to offer an intuitive understanding of the main topics.
### Trend Analysis
**Hashtags Analysis:** The trending hashtags were analyzed over time (weekly and monthly) to identify the popularity and shifts in focus of specific subjects.

**Time-Based Topic Analysis:** LDA was applied to analyze how topics evolved across specific monthly intervals, providing insights into temporal trends within the data.
## Results
The analysis revealed key insights into the nature of discourse on Parler during the specified time frame:
* Clustering Analysis:
  * Optimal Clusters: Through the application of MiniBatchKMeans, an optimal number of clusters were determined that best represented the underlying structure of the data.
  * Themes and Patterns: Different clusters revealed unique themes and patterns, such as political affiliations, sentiments towards specific events, and user behavior.
* Topic Modeling (LDA):
  * Main Topics: LDA identified critical topics that dominated the discourse on Parler. Topics included political events, personalities, and socio-cultural issues.
    * July 2020 - Top Topic: Vote, Trump, Election Campaign
    * November 2020 - Top Topic: Biden, Presidential Election, Breaking News
    * January 2021 - Top Topic: Election Results, Trump, Votes
  * Interactive Visualization: The pyLDAvis tool provided an interactive visualization of the topics, offering a deeper understanding of word associations and topic prevalence.
* Trend Analysis:
  * Trending Hashtags: The analysis of hashtags revealed the top trending tags over time, reflecting shifts in attention and interests.
    * Top Hashtags in July 2020: #MAGA, #Trump2020, #Vote
    * Top Hashtags in January 2021: #StopTheSteal, #Election2020, #Patriots
  * Time-Based Topic Evolution: Monthly LDA analysis showed how the main topics evolved, reflecting changes in public discourse and sentiments.
  * Election Focus: Increase in election-related discussions leading up to November 2020.
  * Post-Election Analysis: Shift towards discussions on election results, legal challenges, and related political events in late 2020 and early 2021.

## Insights:
**Political Landscape:** The analysis provided a snapshot of the political landscape and user behavior on Parler, reflecting the platform's role in shaping public opinion.

**Event-Driven Conversations:** Significant spikes in specific topics and hashtags were observed in response to real-world events, such as elections, protests, and political announcements.

**Temporal Dynamics:** The time-based analysis revealed how conversations evolved, trends emerged, and topics shifted, providing a dynamic view of the discourse on Parler.

## Visualizations
Interactive visualizations were created to represent the clustering and topics, allowing for an engaging exploration of the data.

## Technologies Used
* Python
* Libraries: scikit-learn, pandas, numpy, matplotlib, pyLDAvis
