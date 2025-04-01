# The-Gym-Company-NLP-Topic-Modelling-Project
The Gym Company: NLP Topic Modelling Project

This repository contains the code and documentation for an applied NLP project focused on extracting actionable insights from customer review data. The project was developed for **The Gym Company** (client name anonymized) to help identify and address operational challenges based on automated topic modelling of negative customer reviews.

## Project Overview

In today's highly competitive fitness industry, understanding customer sentiment is crucial for maintaining market leadership. This project leverages automated topic modelling and emotion analysis to uncover key themes in customer reviews sourced from Google and Trustpilot. By focusing on negative and angry reviews, the analysis identifies critical operational pain points and generates specific, actionable recommendations for immediate improvements.

## Problem Statement

Fitness centres face significant operational challenges that directly affect customer satisfaction and retention. The Gym Company, a leading provider of affordable and flexible fitness services, receives extensive feedback from its members through various channels. However, manually sifting through these reviews is inefficient and prone to oversight. This project aims to automate the extraction of key issues—such as facility maintenance, access difficulties, scheduling problems, and poor customer service—from a large volume of negative reviews. By identifying and addressing these challenges, The Gym Company can enhance member satisfaction, optimize operational efficiency, and strengthen its competitive position.

## Sequential Multi-Agentic Workflow

- Our sequential multi-agentic workflow is designed to systematically transform raw customer review data into actionable business insights.

- The process begins with the **Data Ingestion Agent**, which loads and cleans the review data from multiple sources. Next, the **Preprocessing Agent** standardizes the text by converting it to lowercase, removing numbers and stopwords, and tokenizing the content. The **Frequency Analysis Agent** then analyzes the word distributions and creates visualizations, providing an initial overview of dominant terms. Following this, the **Topic Modelling Agent** applies BERTopic (with a comparison to LDA) to extract distinct thematic clusters from negative reviews, while the **Emotion Analysis Agent** isolates reviews expressing anger to pinpoint critical issues. The **LLM-Based Insight Agent** further refines these outputs by generating business-specific recommendations, which are complemented by the **Location Analysis Agent** that identifies hotspots of negative sentiment. Finally, the **Reporting Agent** integrates all these outputs into a comprehensive report, ensuring that each sequential step builds on the previous one to deliver clear, actionable insights for strategic decision-making.

  ![image](https://github.com/user-attachments/assets/4a790622-27b0-4c5a-8a22-2eec82ffe88d)

  
## Key Objectives

- **Data Collection and Preparation:**  
  Loading and cleaning review data from Google and Trustpilot, filtering for negative reviews (ratings/stars below 3) and further isolating those with angry sentiment.
  
- **Frequency Analysis and Visualization:**  
  Perform word frequency analysis and generate visualizations (histograms and word clouds) to identify dominant terms.

- **Topic Modelling:**  
  Use BERTopic (with a comparison to Gensim’s LDA) to extract thematic clusters from the negative reviews. Generate interactive visualizations and analyze key clusters.

- **Emotion Analysis:**  
  Classify review sentiment using a BERT-based model and focus on angry reviews for deeper insight.

- **LLM-Based Insights:**  
  Apply a streamlined language model (sloth φ3.5) to extract actionable topics and generate business-specific recommendations.

- **Location-Based Analysis:**  
  Merge review counts from overlapping locations to identify hotspots where negative feedback is concentrated.

## Business Impact

The insights generated by this project have significant business implications:
- **Enhanced Member Satisfaction:**  
  By identifying and addressing issues related to facility cleanliness, air conditioning, and equipment maintenance, The Gym Company can greatly improve the workout experience. This leads to higher satisfaction and increased member retention.
  
- **Operational Efficiency:**  
  Streamlining access procedures, membership management, and class scheduling not only reduces member frustration but also optimizes resource allocation. The data-driven approach helps pinpoint specific locations with the greatest need for intervention.
  
- **Competitive Advantage:**  
  Implementing targeted improvements based on actionable insights positions The Gym Company as a responsive and member-centric organization. Quick, data-backed adjustments can differentiate the brand in a competitive market.
  
- **Cost Savings and Revenue Growth:**  
  Reducing operational inefficiencies—such as resolving access issues and improving maintenance—can lead to cost savings, while improved customer service and facility quality can drive new memberships and revenue growth.
  
- **Continuous Improvement:**  
  The multi-agent system offers a framework for ongoing monitoring and analysis. This continuous feedback loop ensures that The Gym Company can adapt quickly to changing customer sentiments and maintain market leadership.


