# LEGO Sets Dashboard Report

## Project Overview
This project involves creating an interactive Power BI dashboard to analyze a dataset of LEGO sets. The dashboard provides insights into LEGO themes, price ranges, piece counts, and age recommendations. By visualizing these aspects, it allows for better understanding of the LEGO product range, aiding consumers, collectors, and stakeholders.

---

## Dashboard Overview
![Dashboard](https://github.com/ilhemdjenane/Lego-Sets-Analysis/blob/70e946b5b4064a106beabef25f82d9b246c203d3/Lego%20Dashboard.png)

## Key Objectives
The primary goals of this project include:
- Identifying the most popular LEGO themes and subthemes.
- Analyzing price ranges to highlight affordable and premium options.
- Exploring age recommendations to assist in targeted purchases.
- Understanding the correlation between price, pieces, and target age.

---

## Dataset Description
The dataset includes 18,457 entries detailing LEGO sets. Below are some of the key features:

### Key Columns
- **set_id**: Unique identifier for each LEGO set.
- **name**: Name of the LEGO set.
- **year**: Year of release.
- **theme**: Broad classification of the set.
- **subtheme**: Specific category within the theme.
- **themeGroup**: Higher-level grouping of themes.
- **pieces**: Total number of pieces in the set.
- **agerange_min**: Minimum recommended age for the set.
- **US_retailPrice**: Retail price of the set in USD.
- **category**: Classification of the set type (e.g., normal or special).

### Dataset Cleaning and Preparation
1. **Handling Missing Values**:
   - Rows with critical missing values (e.g., `pieces`, `US_retailPrice`) were filtered out.
   - Non-critical fields (e.g., `subtheme`) were left as-is.

2. **Feature Engineering**:
   - Created a `Price Range` column to group sets into `$`, `$$`, `$$$`, and `$$$$` categories.
   - Grouped `agerange_min` into broader age categories (`5 to 9`, `10 to 14`, etc.).

3. **Data Transformation**:
   - Aggregated metrics for total pieces, average price, and total sets by themes and categories.

---

## Dashboard Design
The dashboard comprises several interactive elements for ease of analysis:

### Key Metrics (KPIs)
- **Total Sets**: 18,457 LEGO sets are included in the dataset.
- **Sum of Pieces**: Over 2 million LEGO pieces are represented.
- **Average Price**: The average retail price for a LEGO set is $45.21.

### Filters and Slicers
- **Theme Group**: Filters to explore categories such as `Classic`, `Licensed`, and `Educational` sets.
- **Theme**: Enables a detailed focus on themes like `Star Wars`, `Harry Potter`, or `Disney`.
- **Age Range**: Filters by categories such as `5 to 9`, `10 to 14`, and others.
- **Price Range**: A slider for selecting sets by price brackets.

### Detailed Table
The table view displays:
- Set Name
- Set ID
- Theme
- Age Range
- Average Pieces
- Average Price
- Price Range

### Design Elements
- Bright, user-friendly layout with interactive slicers and filters.
- Logical arrangement of KPIs, visuals, and detailed tables for clarity.

---

## Key Insights
1. **Popular Themes**:
   - The dataset includes 646 unique themes, with `Star Wars` being the most popular, comprising 1,204 sets.
   - Other top themes include `Harry Potter` and `City`, with over 600 sets each.

2. **Price Distribution**:
   - **$:** Affordable sets priced below $25 represent **4,078 sets (22%)**.
   - **$$:** Mid-range sets ($25–$50) make up **1,665 sets (9%)**.
   - **$$$:** Higher-priced sets ($50–$100) include **827 sets (4%)**.
   - **$$$$:** Premium sets priced above $100 are **412 sets (2%)**.

3. **Age Group Analysis**:
   - For ages **1 to 4**, there are **538 sets** containing a total of **56,000 pieces**, with an average price of **$29**.
   - For ages **5 to 9**, there are **3,338 sets** with over **1 million pieces**, and an average price of **$34**.
   - For ages **10 to 17**, there are **396 sets** with **479,000 pieces**, and an average price of **$113**.
   - For ages **18 and over**, there are **113 sets** with **265,000 pieces**, and an average price of **$197**.

4. **Largest LEGO Sets**:
   - The largest LEGO set is the **World Map**, featuring **11,695 pieces** and priced at **$249.99**.
   - Other notable large sets include:
     - **The Ultimate Battle for CHIMA:** 10,004 pieces.
     - **Eiffel Tower:** 10,001 pieces, priced at **$629.99**.

5. **Yearly Trends**:
   - LEGO releases have steadily increased over time, peaking in **2017 with 840 sets released**.
   - Early years like 1970 had fewer releases, such as **41 sets**.

---

## Tools and Techniques
### Tools
- **Power BI**: For creating visualizations and KPIs.
- **CSV**: Dataset format for importing and analysis.

### Techniques
- **DAX Calculations**: Used to compute custom measures such as average price, total pieces, and counts.
- **Data Modeling**: Established relationships between fields to enable efficient filtering and interaction.

---

## How to Use the Dashboard
1. Clone this repository to your local machine.
2. Open the Power BI file (`LEGO_Dashboard.pbix`) using Power BI Desktop.
3. Ensure the dataset (`lego_sets.csv`) is properly linked.
4. Interact with the dashboard using slicers and filters to explore insights.

---

## Future Improvements
- Incorporate additional datasets, such as customer reviews and regional pricing.
- Add visuals for year-wise trends in LEGO releases by theme.
- Introduce drill-through functionality for detailed subtheme analysis.
- Optimize the dashboard for improved performance with larger datasets.

---

## Conclusion
This LEGO dashboard project demonstrates how data visualization can uncover valuable insights into product trends, customer segmentation, and pricing. From understanding popular themes to analyzing price-piece relationships, this project highlights the versatility of Power BI as a tool for data exploration. Feedback and contributions are welcome!

