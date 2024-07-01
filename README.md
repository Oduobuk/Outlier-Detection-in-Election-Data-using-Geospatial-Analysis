# Outlier-Detection-in-Election-Data-using-Geospatial-Analysis


## Election Data Outlier Detection Using Geospatial Analysis

### Overview
This project focuses on detecting potential outliers in election data using geospatial analysis techniques. The goal is to identify polling units where voting results significantly deviate from neighboring units, which could indicate irregularities or anomalies in the election process.

### Key Steps and Components
1. Dataset Preparation:
   - The dataset is loaded from an Excel file containing election results, including geographical coordinates (latitude and longitude) of each polling unit.

2. Neighbour Identification:
   - Neighboring polling units are identified based on their geographical proximity using a radius (e.g., 1 km).

3. Outlier Score Calculation:
   - For each polling unit, outlier scores are calculated by comparing the voting results (e.g., votes for APC, LP, PDP, NNPP) with those of its neighboring units. The score represents the deviation in votes.

4. Outlier Detection and Reporting:
   - Polling units are sorted by outlier scores to pinpoint significant deviations.
   - Visualizations such as bar charts are generated to illustrate outlier scores for each party.
   - Detailed outlier reports highlight the top outliers, explaining the methodology and findings.

### Tools and Libraries Used
- Python Libraries: pandas, scikit-learn (BallTree), matplotlib
- Additional Tools: tabulate (for tabular formatting in output), and file handling in Python.

 ### Files Included
- Python Script: `election_outlier_detection.py` - Contains the main logic for loading data, calculating scores, detecting outliers, and generating visualizations.
- CSV Files:
  - `neighbours.csv`: Contains data on neighboring polling units.
  - `outlier_scores.csv`: Includes outlier scores calculated for each polling unit.
  - `outlier_results.csv`: Sorted results based on outlier scores.


### Report and Results
- The `outlier_report.txt` provides a detailed methodology, top outliers identified, and insights derived from the analysis.
- Visualizations are saved as PNG files for quick reference and analysis.

