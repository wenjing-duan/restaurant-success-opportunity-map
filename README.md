# Restaurant Success & Opportunity Map

## Overview
This project analyzes Yelp restaurant data in Philadelphia to understand the factors associated with restaurant success and identify potential market opportunities for new restaurants.

The project combines descriptive analysis, feature engineering, machine learning, model interpretation, and business recommendations. Restaurant success was framed as a classification problem using restaurant operating status and rating-based indicators.

## Business Questions
- What factors influence restaurant success in a competitive restaurant market?
- Can restaurant success be predicted using restaurant attributes, customer engagement, and location-related features?
- Where are potential market opportunities for new restaurants?

## Data
The analysis uses Yelp restaurant data filtered for Philadelphia restaurants, including:

- Restaurant attributes such as ratings, location, categories, price range, and operating status
- Customer review data, including ratings, text, and review engagement signals
- Check-in data as a proxy for customer activity
- Demographic variables incorporated at the postal-code level where available

## Tools
- Python
- pandas
- scikit-learn
- Logistic Regression
- Random Forest
- TF-IDF
- NLP
- Feature Engineering
- Data Visualization

## Repository Files
- `restaurant_success_opportunity_map.ipynb`: Python workflow for data preparation, feature engineering, NLP exploration, modeling, and business analysis
- `restaurant_success_opportunity_map_report.pdf`: Polished project report with methodology, model results, visualizations, findings, and recommendations

## Methodology
The project follows a structured analytical workflow:

1. Data preparation and merging  
2. Feature engineering for customer engagement, location, demographics, and restaurant attributes  
3. Exploratory analysis of restaurant performance patterns  
4. Baseline classification using Logistic Regression  
5. Advanced classification using Random Forest  
6. Model evaluation using accuracy, precision, recall, F1 score, and confusion matrices  
7. Model interpretation using feature importance  
8. Business recommendation development based on model and market insights  

## Model Results
Random Forest outperformed the Logistic Regression baseline across key evaluation metrics:

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Logistic Regression | ~68% | ~75% | ~71% | ~0.73 |
| Random Forest | 72.8% | 78.3% | 77.5% | 0.779 |

## Key Findings
- Customer engagement, especially review volume and check-in activity, was one of the strongest predictors of restaurant success.
- Location-related features and neighborhood context contributed meaningfully to restaurant performance.
- Random Forest captured nonlinear relationships better than Logistic Regression.
- Restaurants in high-demand but moderately competitive areas may represent stronger market opportunities.

## Business Recommendations
- Target locations with strong customer demand and moderate competition.
- Prioritize early customer engagement through visibility, reviews, and online presence.
- Monitor customer feedback regularly to improve service quality and retention.
- Differentiate through customer experience rather than relying only on cuisine type or offering.

## Limitations and Future Work
The success definition relies on operating status and rating-based indicators, which do not fully capture revenue, profitability, or customer retention. Future work could incorporate time-series review trends, more advanced NLP methods, more detailed geographic competition features, and external business metrics such as foot traffic or online ordering data.
