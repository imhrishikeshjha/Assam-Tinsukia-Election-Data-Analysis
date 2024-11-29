# Analysis of Candidate Vote Distribution in Assam Elections (1951-2021)

This repository presents a detailed analysis of vote distributions in Assam's elections from 1951 to 2021. It highlights trends, variability, and significant outliers, using advanced data visualization techniques and robust data cleaning strategies.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Data Cleanup Strategy](#data-cleanup-strategy)  
3. [Visualizations](#visualizations)  
4. [Key Findings](#key-findings)  
5. [Temporal Analysis](#temporal-analysis)  
6. [Implications](#implications)  
7. [Data Quality](#data-quality)  
8. [Files](#files)  
9. [Getting Started](#getting-started)  
10. [Contributions](#contributions)  
11. [License](#license)

---

## 1. Project Overview

The primary objectives of this project are:
- To analyze and visualize vote distributions across different election years.
- To identify trends, patterns, and outliers in electoral data.
- To understand the impact of demographic and political changes on vote counts.

---

## 2. Data Cleanup Strategy

A robust data-cleaning process ensures the dataset is consistent and ready for analysis. Key steps include:
- **Handling Missing Data**: Replace missing values with `NaN` and remove rows with "None" in the 'VOTES' column.
- **Standardizing Names**: Clean up assembly constituency and candidate names by removing non-alphabetic characters and excess whitespace.
- **Removing Duplicates**: Ensure unique entries based on key fields like `YEAR`, `AC`, and `CANDIDATE`.
- **Data Type Standardization**: Convert columns like `YEAR` and `VOTES` to their appropriate data types.

---

## 3. Visualizations

The analysis includes the following visualizations:

1. **Box Plot with Outliers (Matplotlib)**: Highlights variability and outliers in vote counts.  
   ![Box Plot](path/to/box_plot_outliers_matplotlib.png)

2. **Violin Plot (Matplotlib)**: Depicts the density and shape of vote distributions.  
   ![Violin Plot](path/to/violin_plot_matplotlib.png)

3. **Box Plot Highlighting Outliers (Altair)**: Focuses on outliers with an interactive, modern approach.  
   ![Altair Box Plot](path/to/box_plot_altair.png)

---

## 4. Key Findings

1. **Rising Vote Counts**: A significant increase in median and maximum vote counts, especially post-2001.  
2. **Greater Variability**: The interquartile range (IQR) has widened over time.  
3. **Emergence of Outliers**: High-performing outliers have grown in number and intensity.  
4. **Skewed Distributions**: Early years were more symmetrical; recent years show long upper tails.

---

## 5. Temporal Analysis

- **1951-1983**: Stable and compact distributions.  
- **1985-2000**: Gradual increase in vote counts and variability.  
- **2001-2021**: Marked by high variability and a surge in outliers.

---

## 6. Implications

1. **Electoral Competitiveness**: More candidates securing high votes indicate dynamic competition.  
2. **Changing Political Landscape**: Strong regional parties and shifts in voter behavior play a key role.  
3. **Demographics**: Population growth and turnout significantly influence trends.

---

## 7. Data Quality

1. **Improved Reporting**: Enhanced data accuracy in recent years.  
2. **Detailed Distributions**: More granular details in modern election data aid analysis.

---

## 8. Files

- `TDSp1.ipynb`: Analysis code in Jupyter Notebook.  
- `RESULT INFERENCE.docx`: Detailed observations document.  
- `_Data Cleanup Strategy.docx`: Data cleanup steps.  
- Visualization images: Available in the `images/` folder.

---

## 9. Getting Started

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/assam-election-analysis.git
pip install -r requirements.txt
jupyter notebook TDSp1.ipynb

10. Contributions
Contributions are welcome! Fork this repository, make improvements, and submit pull requests.

