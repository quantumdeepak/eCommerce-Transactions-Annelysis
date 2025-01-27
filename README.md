# eCommerce-Transactions-Annelysis
# Customer Analysis and Segmentation Project

## Overview
This project analyzes customer behavior, product sales patterns, and customer segmentation using transaction data. The analysis includes lookalike modeling and customer clustering to identify distinct customer segments.

## Data Sources
The project uses three main datasets:
- `Customers.csv`: Customer information including ID, name, signup date, and region
- `Products.csv`: Product details including ID, name, and category
- `Transactions.csv`: Transaction records with customer purchases

## Analysis Components

### 1. Product Sales Analysis
- Analyzed monthly sales patterns for different products
- Examined product category performance across regions
- Investigated day-of-week sales patterns
- Key findings:
  - Sales data remains consistent throughout the year
  - Home decor items show higher sales on Saturdays
  - Book sales peak on Wednesdays
  - Sales patterns vary significantly by region

### 2. Lookalike Model
- Implemented a customer similarity model using cosine similarity
- Features used:
  - Purchase quantities by product category
  - Total spending
  - Customer demographics
- Created normalized similarity scores for better comparison
- Generated top 3 lookalike customers for each customer

### 3. Customer Segmentation
- Implemented clustering using K-means algorithm
- Optimized cluster count using Davies-Bouldin Index
- Key findings:
  - Optimal number of clusters: 9
  - Used PCA for dimensionality reduction
  - Achieved improved Davies-Bouldin score after optimization
  - Each cluster shows distinct purchasing patterns and regional preferences

## Key Findings
1. Sales Patterns:
   - Consistent sales throughout the year
   - Category-specific day-of-week preferences
   - Regional variations in product popularity

2. Customer Segments:
   - Identified 9 distinct customer segments
   - Each segment shows unique purchasing behaviors
   - Clear regional preferences within segments

## Files Generated
- `Lookalike.csv`: Contains lookalike recommendations for customers
- `segmented_customers_with_pca.csv`: Customer segmentation results

## Technical Implementation
- Used Python with pandas, scikit-learn, and numpy
- Implemented various machine learning techniques:
  - K-means clustering
  - PCA dimensionality reduction
  - Cosine similarity calculations
- Visualization using matplotlib and seaborn

## Future Improvements
- Consider implementing more sophisticated clustering algorithms
- Add seasonal analysis for better trend detection
- Include more customer demographic features in segmentation
- Explore alternative similarity metrics for lookalike modeling
