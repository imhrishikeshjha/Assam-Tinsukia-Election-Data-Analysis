
# Analysis of Candidate Vote Distribution in Assam Elections (1951-2021)

This project explores the evolution of vote distributions in Assam's elections from 1951 to 2021. By analyzing historical election data, we uncover trends, patterns, and key insights using advanced data visualization techniques.

## Project Overview

The main objectives of this project are:
- To visualize vote distributions across different election years.
- To identify trends and patterns, such as increasing vote counts, variability, and outliers.
- To understand the impact of demographic, political, and electoral changes.

## Data Cleanup Strategy

To ensure the data is consistent and reliable for analysis, the following steps were undertaken:

1. **Handling Missing Data**:
   - Replace empty strings with NaN values for consistency.
   - Remove rows where 'VOTES' is "None" to ensure data integrity.

2. **Assembly Constituency (AC) Name Cleanup**:
   - Strip leading numbers and spaces (e.g., "01 Constituency" becomes "Constituency").
   - Remove non-alphabetic characters, except spaces and periods, to standardize names.

3. **Candidate Name Cleanup**:
   - Similar to AC names, remove leading numbers and spaces.
   - Eliminate non-alphabetic characters (excluding spaces and periods) for consistency.

4. **Whitespace Management**:
   - Trim excess whitespace from all string columns to improve data quality.

5. **Duplicate Entry Removal**:
   - Perform initial removal of all duplicate rows.
   - Conduct targeted de-duplication based on key fields (ST_NAME, YEAR, AC, CANDIDATE, SEX, AGE, CATEGORY, PARTY, VOTES) to maintain unique election entries.

6. **Data Type Standardization**:
   - Treat all data as strings during the cleaning process for consistent handling.
   - Convert specific columns to appropriate data types (e.g., YEAR to integer, VOTES to float) for analysis.

7. **Data Saving Approach**:
   - Save complete state data to a CSV file.
   - Filter and save data for specific Assembly Constituencies separately for focused analysis.

8. **Error Management**:
   - Implement checks to verify state data existence before proceeding with scraping and cleaning.
   - Provide appropriate feedback if data is unavailable for a given state.

This strategy ensures a robust dataset suitable for in-depth electoral studies by addressing missing data, inconsistent naming conventions, and duplicates.

## Visualizations

The project leverages Matplotlib and Altair to create meaningful visualizations, including:

1. **Box Plot with Outliers (Matplotlib)**  
   Highlights variability and outliers in vote counts.  
   ![Box Plot with Outliers](path/to/box_plot_outliers_matplotlib.png)

2. **Violin Plot (Matplotlib)**  
   Shows the density and shape of vote distributions.  
   ![Violin Plot](path/to/violin_plot_matplotlib.png)

3. **Box Plot Highlighting Outliers (Altair)**  
   Focuses on outliers with a modern visualization approach.  
   ![Box Plot (Altair)](path/to/box_plot_altair.png)

## Key Findings

1. **Trends in Vote Counts**  
   - A significant upward trend in median and maximum vote counts, especially after 2001.

2. **Increasing Variability**  
   - The interquartile range has widened over time, reflecting greater variability.

3. **Emergence of Outliers**  
   - Noticeable growth in the number and extremity of outliers, particularly in 2016 and 2021.

4. **Changing Distribution Patterns**  
   - Early years show compact distributions, while recent years are skewed with long tails.

## Temporal Analysis

1. **1951-1983**  
   Stable and compact distributions.  
2. **1985-2000**  
   Gradual increase in variability and vote counts.  
3. **2001-2021**  
   Dramatic changes in patterns, with notable outliers.

## Implications

- **Electoral Competitiveness**: Increased range and high-performing candidates indicate dynamic competition.  
- **Political Landscape**: The rise of regional parties and shifts in voter behavior contribute to observed trends.  
- **Demographic Factors**: Population growth and voter turnout influence the transformations.

## Data Quality

- Improved data collection over time enhances the accuracy of analyses.
- Detailed distributions in recent elections reflect advancements in reporting.

## Comparative Insights

- Box plots and violin plots offer complementary views, balancing simplicity and density visualization.
- Altair's box plot highlights outliers effectively, aiding focused analyses.

## Files

- `TDSp1.ipynb`: The Jupyter notebook containing the analysis code.  
- `RESULT INFERENCE.docx`: Detailed results and observations document.  
- `_Data Cleanup Strategy.docx`: Document outlining the data cleanup strategy.  
- Visualization images: Located in the `images/` folder.

## Getting Started

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/assam-election-analysis.git
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook for exploration:  
   ```bash
   jupyter notebook TDSp1.ipynb
   ```

## Contributions

Feel free to fork this repository and submit pull requests for improvements or additional insights.

## License

This project is licensed under the [MIT License](LICENSE).
