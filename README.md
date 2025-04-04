# Learning Tableau

## Table of Contents

- [Installing Tableau and Creating Your First Visualization](#installing-tableau-and-creating-your-first-visualization)
  - [Installing Tableau Public](#installing-tableau-public)
  - [Connecting to a Dataset](#connecting-to-a-dataset)
  - [Creating Basic Visualizations](#creating-basic-visualizations)
- [Using Joins in Tableau](#using-joins-in-tableau)
  - [Understanding Joins vs. Relationships](#understanding-joins-vs-relationships)
  - [Types of Joins in Tableau](#types-of-joins-in-tableau)
- [Creating Visualizations](#creating-visualizations)
  - [Common Charts in Tableau](#common-charts-in-tableau)
- [Using Calculated Fields and Bins](#using-calculated-fields-and-bins)
  - [Bins](#bins)
  - [Calculated Fields](#calculated-fields)
- [Summary](#summary)


## Installing Tableau and Creating Your First Visualization

### Installing Tableau Public

- Tableau Public is a free version of Tableau with limited features but ideal for learning and portfolio building.
- Steps to install:
    1. Download from Tableau Public's official website: https://www.tableau.com/products/public
    2. Provide an email and install the application.
    3. Open Tableau Public and navigate the interface.

### Connecting to a Dataset

- Use the **Video Game Sales** dataset from Kaggle for practice: https://www.kaggle.com/datasets/gregorut/videogamesales
- Load the dataset by selecting **Text File** in Tableau.
- Tableau automatically categorizes data types (numeric, text, date).

### Creating Basic Visualizations

- **Line Chart:**
    - Import the video game sales CSV into Tableau Public and open a new worksheet.
    - Drag the `Global Sales` measure onto the Rows shelf and the `Year` dimension onto the Columns shelf to create a basic line graph.
    - Add the `Genre` dimension to the Marks card under Color to visually differentiate each game genre.
    - Include labels for min and max values along the lines to provide additional context.
- **Genre Sales Chart:**
    - Open another worksheet to focus on overall sales by game genre.
    - Set `Genre` as your primary dimension and `Global Sales` as the measure.
    - Use the sorting feature to organize the data and assign distinct colors to each genre for clarity.
    - Finally, combine these worksheets into a dashboard for a comprehensive view.

![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image.png)

## Using Joins in Tableau

Download excel file: https://github.com/AlexTheAnalyst/PortfolioProjects/blob/main/Tableau%20Joins%20File.xlsx

### Understanding Joins vs. Relationships

- Tableau uses **Relationships** by default, which dynamically infer joins based on data.
- **Joins** allow more control over how tables merge.

### Types of Joins in Tableau

- **Inner Join:** Includes only matching records between tables.
- **Left Join:** Includes all records from the left table and matches from the right.
- **Right Join:** Includes all records from the right table and matches from the left.
- **Full Outer Join:** Includes all records from both tables.

![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%201.png)

## Creating Visualizations

Download this dataset: https://www.kaggle.com/datasets/starbucks/store-locations

### Common Charts in Tableau

- **Bar and Line Graphs:** Combine bars and lines for comparative sales analysis.
    
    ![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%202.png)
    
- **Maps:** Use geographic data (longitude/latitude) to create density or filled maps.
    - Import **Starbucks store locations** dataset.
    - Drag `Latitude` and `Longitude` into **Columns** and **Rows**.
    - Use **State** or **Postal Code** as a level of detail.
        
        ![Store location density by zipcode.](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%203.png)
        
        Store location density by zipcode.
        
- **Scatter Plots:** Compare two numeric fields to analyze correlations.
    
    ![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%204.png)
    

## Using Calculated Fields and Bins

### **Bins**

- Bins group numeric data into defined ranges (e.g., 1990–1994, 1995–1999).
- To create bins, right-click a numeric field (such as `Year`) and select **Create → Bins**, then choose a bin size (e.g., 5).
- Bins turn continuous numeric values into categories, making it easier to compare grouped data (for instance, total sales per 5-year range).
- You can exclude null or unwanted values from the view if needed (e.g., by right-clicking on null bars and selecting **Exclude**).

![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%205.png)

### **Calculated Fields**

- Calculated fields let you build new measures or dimensions from existing data (e.g., `[Global Sales] - [EU Sales]`).
- To create one, click the dropdown next to a field, choose **Create → Calculated Field**, then enter your formula.

![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%206.png)

- Quick table calculations (like “Percent of Total”) are built-in options, and you can drag them into the data pane to save them as custom fields.

![image.png](https://github.com/ndomah1/Learning-Tableau/blob/main/images/image%207.png)

- Use calculated fields to perform basic arithmetic, combine fields, or handle more complex logic, depending on your analysis needs.

## Summary

These tutorials provide a foundational understanding of Tableau, covering installation, joins, visualization types, and calculations. For a deeper understanding, practicing with real-world datasets and different chart types is recommended.
