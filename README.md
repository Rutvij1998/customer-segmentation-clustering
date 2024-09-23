# Customer Segmentation Using K-Means Clustering

## Project Description

This project focuses on segmenting customers based on their demographic and spending behavior using **K-Means Clustering**. The goal is to classify customers into distinct groups that share similar characteristics, such as **age**, **annual income**, and **spending score**. This type of analysis is highly valuable for businesses to identify different types of customers and tailor marketing strategies to target each segment effectively.

### Objective

The main objective of this project is to:
- Apply unsupervised learning techniques (K-Means) to create meaningful customer segments.
- Analyze customer behavior by visualizing patterns in age, income, and spending.
- Provide business insights that can help companies optimize their customer engagement strategies.

### Dataset Description
- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer (not used in clustering).
- **Age**: Age of the customer.
- **Annual Income (k$)**: The annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: A score that represents how much a customer spends.

### Methodology

1. **Data Preprocessing**:
   - The data is first cleaned by handling missing values and converting categorical columns (like `Gender`) into a usable format.
   - The relevant features for clustering are **Age**, **Annual Income**, and **Spending Score**.

2. **Feature Scaling**:
   - We scale the selected features using **MinMaxScaler** to bring them to a common scale, which is necessary for distance-based clustering algorithms like K-Means.

3. **K-Means Clustering**:
   - Using the **Elbow Method**, the optimal number of clusters is identified by analyzing the sum of squared errors (SSE).
   - The K-Means algorithm is then applied to segment customers into distinct groups based on their similarities.

4. **Visualization**:
   - 2D scatter plots and a 3D scatter plot are used to visualize the clusters.
   - Visualizations help to better understand the relationships between variables like **Annual Income** and **Spending Score**, revealing patterns among different customer groups.

5. **Cluster Evaluation**:
   - The quality of the clusters is evaluated using the **silhouette score**, a metric that measures how well the customers are clustered.

### Key Insights

- **High-Income, High-Spending Customers**: This group can be targeted for premium product offerings and loyalty programs.
- **Low-Income, High-Spending Customers**: These customers may benefit from installment plans or rewards for continued loyalty.
- **Young Customers with High Spending Scores**: These customers might be more inclined to try new products and could be targeted with early-bird promotions.
- **Low-Income, Low-Spending Customers**: Businesses may want to focus on budget-friendly offerings and personalized discounts for this group.

### Visualizations
The project includes various plots:
- **2D Scatter Plots**: Visualizing the relationship between variables like **Age vs. Spending Score** and **Annual Income vs. Spending Score**.
- **3D Scatter Plot**: Offering a detailed view of how customers cluster across all three variables.

### Technologies Used
- **Python**: For data analysis and visualization.
- **Pandas, NumPy**: For data manipulation and cleaning.
- **Seaborn, Matplotlib**: For plotting and visualizing the results.
- **Scikit-learn**: For K-Means clustering and scaling.
- **Jupyter Notebook**: For interactive coding and visual output.

### How to Run the Project
1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd customer-segmentation-clustering
