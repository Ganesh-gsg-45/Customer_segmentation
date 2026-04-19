# Customer Segmentation Project

This project performs customer segmentation using the Online Retail II dataset. It uses RFM analysis and K-Means clustering to group customers into segments, then saves the clustered results for further analysis.

## Project Structure

- `data/raw/online_retail_II.xlsx` - source dataset file
- `notebook/eda.ipynb` - main Jupyter notebook with data cleaning, analysis, clustering, and visualization
- `notebook/clustered_customers.csv` - exported customer clustering results
- `notebook/cluster_summary.csv` - exported cluster summary metrics
- `requirements.txt` - required Python packages
- `.gitignore` - files and folders excluded from Git
- `README.md` - project documentation

## Requirements

Install the required packages with:

```bash
pip install -r requirements.txt
```

## How to Run

1. Open `notebook/eda.ipynb` in Jupyter Notebook or JupyterLab.
2. Run the cells in order from top to bottom.
3. The notebook reads the dataset, cleans the data, builds RFM features, scales the data, applies K-Means clustering, and visualizes the cluster results.
4. After running, the outputs will be saved as CSV files in the `notebook/` folder.

## Notes

- The notebook uses a relative path to load the dataset from `../data/raw/online_retail_II.xlsx`.
- If your environment is different, update the file path accordingly.
- You can adjust the number of clusters in the notebook by changing `k` in the clustering cell.

## Recommended Next Steps

- Review cluster labels and adjust segment names based on cluster statistics.
- Add model validation metrics such as silhouette score.
- Create a separate Python script for automation or a dashboard for visualization.
