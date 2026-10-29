
# 📊 Retail Sales Analytics Dashboard Using Graph Analytics

## 📌 Project Overview

The **Retail Sales Analytics Dashboard** is a Python-based data analytics project designed to analyze retail sales data and visualize important business insights through an interactive web dashboard.

The project helps businesses understand sales performance, profit trends, customer purchasing behavior, product performance, and regional sales distribution. It also uses **Graph Analytics** to explore relationships between customers and products.

The dashboard is developed using Streamlit and provides interactive charts, key performance indicators (KPIs), filtering options, and dataset download functionality.

## 🎯 Objectives

- Analyze retail sales and profit performance.
- Identify top-selling products and profitable product categories.
- Understand monthly sales trends.
- Compare sales performance across different regions.
- Analyze customer–product relationships using graph analytics.
- Identify highly connected products using degree centrality.
- Present business insights through an interactive dashboard.

## ✨ Features

### 1. Key Performance Indicators (KPIs)
Displays essential business metrics:

- Total Sales
- Total Profit
- Total Orders
- Total Customers
- Total Quantity Sold

### 2. Monthly Sales Analysis
Visualizes monthly sales trends to understand changes in sales performance over time.

### 3. Category-Wise Sales Analysis
Compares sales and profit across different product categories.

### 4. Regional Sales Analysis
Identifies regions with higher and lower sales performance.

### 5. Top 10 Products
Displays the ten products generating the highest total sales.

### 6. Sales vs. Profit Analysis
Visualizes the relationship between sales revenue and profit across product categories.

### 7. Customer–Product Graph Analytics
Creates a network graph representing relationships between customers and products.

- **Nodes:** Customers and products.
- **Edges:** Relationships between customers and products they purchased.
- **Degree Centrality:** Helps identify highly connected nodes and products.

### 8. Interactive Filters
Users can filter dashboard data by:

- Region
- Product Category
- Customer Segment

The dashboard updates its visualizations based on the selected filters.

### 9. Dataset Preview and Download
Allows users to view filtered sales records and download the filtered dataset as a CSV file.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical calculations |
| Plotly | Interactive data visualizations |
| NetworkX | Graph creation and network analysis |
| Streamlit | Interactive web dashboard |
| Matplotlib | Data visualization |
| Google Colab | Development and execution environment |
| Cloudflare Tunnel | Temporary public access to the locally running application |

## 📂 Project Structure

```text
Retail-Sales-Analytics/
│
├── app.py                       # Streamlit dashboard application
├── retail_sales_cleaned.csv     # Cleaned retail sales dataset
├── README.md                    # Project documentation
└── requirements.txt             # Python dependencies
```

*Note: The CSV dataset and requirements file should be included in the repository if you intend to distribute them. The dataset filename must match the filename used in `app.py`.*

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.9 or later
- pip package manager
- A retail sales dataset in CSV format

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd Retail-Sales-Analytics
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### Step 2: Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly networkx openpyxl streamlit
```

### Step 3: Prepare the Dataset

Place the cleaned dataset in the project directory and name it:

```text
retail_sales_cleaned.csv
```

Ensure that the dataset contains the columns required by the application, including sales, profit, quantity, order date, order ID, customer ID, product ID, product name, region, category, and customer segment.

### Step 4: Run the Application

```bash
streamlit run app.py
```

### Step 5: Open the Dashboard

Open the local URL displayed in your terminal, usually:

```text
http://localhost:8501
```

The dashboard will open in your web browser.

## 📊 Dashboard Insights

The dashboard enables users to explore questions such as:

- Which products generate the highest sales?
- Which regions contribute the most revenue?
- How do sales change from month to month?
- Which product categories generate higher profits?
- Which products have the most customer connections?
- How do sales and profit vary across product categories?

The insights depend on the dataset provided to the application.

## 🧠 Graph Analytics Methodology

The project uses NetworkX to create a customer–product network.

1. Select frequently occurring customers from the filtered dataset.
2. Create customer and product nodes.
3. Connect customers to the products they purchased.
4. Calculate node degree and degree centrality.
5. Visualize the network and identify highly connected products.

This approach provides a network-based view of purchasing relationships and complements traditional sales charts.

## 🚀 Future Enhancements

- Add sales forecasting using machine learning.
- Develop a product recommendation system.
- Implement market basket analysis and association rules.
- Add customer segmentation using clustering algorithms.
- Include date-range filters and advanced reporting.
- Deploy the dashboard on a cloud hosting platform.

## 💡 Applications

- Retail business performance monitoring
- Sales and profit analysis
- Product performance evaluation
- Customer purchasing relationship analysis
- Data-driven business decision-making

## 👩‍💻 Conclusion

The Retail Sales Analytics Dashboard combines traditional retail data analysis with graph analytics to provide a comprehensive view of business performance. By integrating data processing, interactive visualizations, and customer–product relationship analysis, the project helps users explore sales patterns and identify useful business insights through a single web application.

---

**Project Title:** Retail Sales Analytics Dashboard Using Graph Analytics

**Domain:** Data Science and Business Analytics

**Built With:** Python, Pandas, NumPy, Plotly, NetworkX and Streamlit
