# Customer Segmentation with KMeans Clustering

## Overview
This project demonstrates a hands-on approach to customer segmentation using **KMeans Clustering** in Python. The goal is to provide actionable insights into customer behavior for an online retail business. By leveraging the **RFM (Recency, Frequency, Monetary)** model and clustering techniques, we classify customers into meaningful groups to aid business decision-making.

## Features
- **Data Exploration**: Handling missing data, outliers, and inspecting key features like Invoice Numbers, Stock Codes, and Customer IDs.
- **Data Cleaning**: Filtering out invalid or irrelevant data points to ensure accurate analysis.
- **Feature Engineering**: Calculating RFM features from transactional data.
- **Clustering Analysis**: Applying KMeans clustering and evaluating results using the Elbow Method and Silhouette Scores.
- **Visualization**: Insights through 3D plots, violin plots, and cluster labeling.

## Project Highlights
- **Dataset**: [Online Retail II Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II) (2009-2011 UK-based retail transactions).
- **Tools Used**:
  - Python
  - Pandas, NumPy
  - Matplotlib, Seaborn
  - Scikit-learn
  - OpenPyXL

## Workflow
1. **Exploratory Data Analysis (EDA):**
   - Understanding data structure (columns like Invoice Number, Stock Code, Quantity, Unit Price, Customer ID, etc.).
   - Dealing with missing values and inconsistencies (e.g., negative prices or quantities).

2. **Data Cleaning:**
   - Removing null Customer IDs and irrelevant invoice types (e.g., cancellations or accounting entries).
   - Addressing outliers in Quantity, Unit Price, and Stock Codes.

3. **Feature Engineering:**
   - Creating RFM metrics:
     - **Recency**: Days since the last purchase.
     - **Frequency**: Number of purchases.
     - **Monetary**: Total spending.
   - Scaling data to standardize features for clustering.

4. **Clustering Analysis:**
   - Using the **Elbow Method** to determine the optimal number of clusters.
   - Validating cluster quality with **Silhouette Scores**.
   - Assigning meaningful labels to clusters (e.g., Retain, Reward, Nurture, Re-engage).

5. **Visualization:**
   - 3D scatter plots to visualize clusters.
   - Violin plots for distribution analysis of RFM metrics.

## Results
### Sample Outputs:
- **3D Cluster Visualization:**
  ![Cluster Plot Example](https://github.com/user-attachments/assets/498e79c1-d414-40ad-a424-b1caf32ebade)

- **Violin Plots of RFM Metrics:**
  ![Violin Plot Example](https://github.com/user-attachments/assets/1048f19c-25a1-42d8-8df8-500f85a145d5)
  ![Violin Plot Example](https://github.com/user-attachments/assets/27a5ac05-cfb1-49ad-9787-2dc0dde043ee)

- **Cluster Distribution with Average Feature Values:**
  ![Combine Visual Chart](https://github.com/user-attachments/assets/de2ea261-e2d0-4504-855f-c7e53d6ca81f)

## Getting Started
### Prerequisites
1. Python 3.7+
2. Required Libraries:
   ```bash
   pip install -r requirements.txt
   ```

### Dataset
Download the dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II) and place it in the `data/` folder.

### Running the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/kmeans-clustering.git
   cd kmeans-clustering
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter notebook:
   ```bash
   jupyter notebook online_retail_data_clustering.ipynb
   ```
4. Run all cells to see the analysis.

## Project Structure
```
|-- data/
|   |-- OnlineRetail_2009-2010.xlsx
|-- notebooks/
|   |-- online_retail_data_clustering.ipynb
|-- requirements.txt
|-- README.md
```

## Challenges
- Handling large datasets with over 500,000 records.
- Dealing with data inconsistencies, such as cancellations and invalid values.
- Optimizing cluster selection to balance granularity and interpretability.

## Future Work
- Extend analysis to include geolocation data (e.g., customer countries).
- Automate cluster labeling using advanced NLP techniques.
- Deploy clustering results to a dashboard for real-time business insights.

## Acknowledgments
- Inspired by Trent's tutorial on clustering techniques.
- Dataset from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II).

## License
This project is licensed under the [MIT License](LICENSE).

---
For any questions or suggestions, feel free to contact me via GitHub or open an issue!
