# openai_reviews_analysis

# Yelp House Cleaning Reviews Analysis with OpenAI

## Purpose
This repository contains a pipeline for automated analysis of customer reviews of a house cleaning service. The goal is to:

- Extract structured positive and negative feedback categories and subcategories from free-form text  
- Aggregate and visualize frequency of each feedback category  
- Generate a concise summary of top features and pain points with representative quotes  

## Data Preprocess ('openai_reviews_analysis_yelp.ipynb')
   - Read raw CSV of reviews (`House Cleaning Reviews.csv`)  
   - Prompt OpenAI’s GPT-4o-mini to return JSON arrays of positive/negative categories and subcategories for each review  
   - Parse JSON and store results in a pandas DataFrame  
   - Count frequencies of each category (positive vs. negative)  
   - Plot a grouped bar chart sorted by total mentions  
   - Get a single summary from GPT-4o-mini, include frequency, brief explanation, and one representative quote per item  

## Technologies Used
- **Python 3.8+**  
- **pandas** for data manipulation  
- **openai-python** SDK (v1.0+) for GPT API calls you need your own API key
- **matplotlib** for plotting  
- **JSON** for structured data exchange  
