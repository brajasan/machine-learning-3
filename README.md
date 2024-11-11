# Restaurant Recommendation Engine

## Overview
The Restaurant Recommendation Engine is a Python-based project that utilizes data from Yelp to recommend restaurants based on user location and preferences. The project employs data analysis and machine learning techniques, specifically K-Means clustering, to categorize restaurants and provide recommendations.

## Features
- Load and preprocess restaurant data from a JSON file.
- Perform exploratory data analysis (EDA) to visualize restaurant ratings and distributions.
- Implement K-Means clustering to group restaurants based on geographical coordinates.
- Recommend top restaurants based on user location and clustering results.
- Visualize restaurant locations and clusters on interactive maps using Plotly and Folium.

## Requirements
To run this project, you need the following Python libraries:
- pandas
- numpy
- geopandas
- matplotlib
- seaborn
- folium
- plotly
- scikit-learn

You can install the required libraries using pip:

```bash
pip install pandas numpy geopandas matplotlib seaborn folium plotly scikit-learn
```

## Usage
1. **Load the Dataset**: The dataset is loaded from a JSON file named `yelp_academic_dataset_business.json`. Ensure this file is in the same directory as the notebook.

2. **Exploratory Data Analysis**: The notebook includes sections for visualizing the distribution of restaurant ratings and identifying top-rated restaurants.

3. **K-Means Clustering**: The project filters restaurants based on their geographical coordinates and applies K-Means clustering to categorize them.

4. **Recommendation Function**: The `recommend_restaurants` function predicts the cluster for a given user location and returns the top 5 restaurants in that cluster.

5. **Map Visualization**: The `recommend_and_plot_map` function generates an interactive map displaying the user's location and recommended restaurants.

## Example
To recommend restaurants based on a specific location, you can use the following code snippet:

```python
longitude = -75.1652 # Example longitude
latitude = 39.9526 # Example latitude
recommended = recommend_restaurants(top_restaurants_pa, longitude, latitude, kmeans)
print(recommended)
```


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Data sourced from Yelp's academic dataset https://www.kaggle.com/datasets/yelp-dataset/yelp-dataset?resource=download.