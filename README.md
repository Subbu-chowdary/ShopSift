# ShopSift

**ShopSift** is a robust data analytics project designed to analyze customer purchase data. By leveraging the Apriori algorithm for market basket analysis and K-Means clustering for customer segmentation, ShopSift enables businesses to gain actionable insights from transaction data. The project outputs interactive 3D visualizations in HTML format, facilitating the exploration of purchase patterns and aiding in optimizing marketing strategies.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Data Format](#data-format)
- [How It Works](#how-it-works)
- [Analysis Overview](#analysis-overview)
  - [Apriori Algorithm](#apriori-algorithm)
  - [K-Means Clustering](#k-means-clustering)
- [Visualization Results](#visualization-results)
- [Use Cases](#use-cases)
- [License](#license)

## Features
- **Market Basket Analysis**: Identify frequently purchased product combinations using the Apriori algorithm.
- **Customer Segmentation**: Segment customers based on their purchasing behavior using K-Means clustering.
- **Interactive Visualizations**: Generate 3D visualizations in HTML for easy analysis and sharing with stakeholders.
- **Scalability**: Adaptable to various types of transactional data, making it a versatile tool for any data-driven organization.

## Installation

### Prerequisites
Ensure you have Python 3.7 or higher installed on your machine. You can download Python from the [official website](https://www.python.org/downloads/).

### Required Packages
To install the necessary packages, open your terminal or command prompt and run the following command:

```bash
pip install numpy pandas faker plotly scikit-learn

```



## Project Overview

ShopSift operates by generating synthetic customer purchase data or loading existing transaction data from a CSV file. The analysis includes the following steps:

1. **Data Generation/Loading**: Synthetic data can be generated using the Faker library, or you can load your own CSV file with transaction data.

2. **Data Preprocessing**: The loaded data is transformed into a binary matrix where rows represent customers and columns represent products. Each cell indicates whether a customer purchased a particular product (1) or not (0).

3. **Market Basket Analysis with Apriori Algorithm**:
   - The Apriori algorithm scans the binary matrix to identify frequent itemsets (combinations of products that are commonly purchased together).
   - It calculates support and confidence for these itemsets, generating association rules that indicate relationships between products.

4. **Customer Segmentation with K-Means Clustering**:
   - The binary matrix is scaled and used as input for the K-Means clustering algorithm, which groups customers into distinct clusters based on their purchasing patterns.

5. **Visualization**: The results of both analyses are visualized using Plotly, producing interactive 3D scatter plots that allow users to explore the relationships between products and understand customer segments effectively.

## Key Features
- **Market Basket Analysis**: Identify frequently purchased product combinations using the Apriori algorithm.
- **Customer Segmentation**: Segment customers based on their purchasing behavior using K-Means clustering.
- **Interactive Visualizations**: Generate 3D visualizations in HTML for easy analysis and sharing with stakeholders.

By utilizing ShopSift, businesses can uncover valuable insights into customer behavior, optimize marketing strategies, and ultimately enhance their sales performance.
