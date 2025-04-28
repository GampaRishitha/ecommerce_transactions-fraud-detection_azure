
# E-commerce Fraud Detection Project using Microsoft Azure

## Overview

This project demonstrates a **Fraud Detection System** for e-commerce transactions using **Azure Data Lake**, **Azure Synapse Analytics**, and **Power BI**. The goal is to identify fraudulent transactions by analyzing transaction data, processing it in Azure Synapse, and visualizing the results using Power BI.

The project follows these steps:
1. **Data Storage**: Store raw transaction data in **Azure Data Lake**.
2. **Data Processing**: Use **Azure Synapse Analytics** to run SQL queries and identify fraudulent transaction patterns.
3. **Data Visualization**: Use **Power BI** to visualize the fraud detection results, including alerts and trends.

## Technologies Used
- **Azure Data Lake**: For storing and managing large datasets in a secure, scalable environment.
- **Azure Synapse Analytics**: For querying and processing large datasets and performing fraud detection.
- **Power BI**: For creating dashboards to visualize fraud patterns and alert users to suspicious activities.

## Project Structure
The project is organized into the following folders:
- `SQL_Scripts/`: Contains SQL queries for fraud detection and data processing in Azure Synapse.
- `Power_BI_Reports/`: Contains Power BI files (.pbix) and screenshots of dashboards used for visualizing the results.
- `Data/`: Contains sample data files, including transactional data and fraud detection results.
- `Documentation/`: Includes this `README.md`, project overview, and architecture diagrams.

## Setup Instructions

### Prerequisites
Before running this project, ensure you have the following:
- An **Azure Subscription** with access to **Azure Data Lake** and **Azure Synapse Analytics**.
- **Power BI Desktop** installed on your machine to view the reports.
- Access to **Azure Synapse Analytics** workspace and connection credentials.

### Step 1: Setup Azure Data Lake
1. Create an **Azure Data Lake** storage account.
2. Upload your raw transactional data (in CSV format) to a container in the Data Lake.

### Step 2: Setup Azure Synapse Analytics
1. Create a **Synapse Workspace** in Azure.
2. Create an **External Data Source** in Synapse to point to the Azure Data Lake location where your data is stored.
3. Create **External Tables** in Synapse to query the transactional data stored in the Data Lake. Use the provided SQL scripts in the `SQL_Scripts/` folder to create external data sources and tables.

### Step 3: Run SQL Queries in Synapse
1. Use the SQL scripts in the `SQL_Scripts/` folder to perform data cleaning and fraud detection.
2. Queries can be run using **Azure Synapse Studio**.

### Step 4: Visualize Data in Power BI
1. Open **Power BI Desktop**.
2. Load the processed data from Azure Synapse into Power BI.
3. Create **visualizations** like bar charts, heatmaps, and line graphs to show fraud patterns, suspicious transactions, and alerts.
4. Save and publish the Power BI report to your Power BI workspace (if required).

## Files in This Repository

### SQL Scripts
- **fraud_detection_queries.sql**: SQL scripts for processing and detecting fraud patterns in the transactional data.
- **data_cleaning_queries.sql**: SQL queries for cleaning and transforming the raw data before analysis.

### Power BI Reports
- **fraud_detection_dashboard.pbix**: Power BI dashboard file containing the visualizations and alerts for fraud detection.
- **fraud_detection_screenshot_1.png**: Screenshot of the first Power BI visualization (fraud detection trends).
- **fraud_detection_screenshot_2.png**: Screenshot of the second Power BI visualization (suspicious transactions by region).

### Data Files
- **sample_transactions_data.csv**: A small sample of transactional data used for fraud detection.
- **sample_fraudulent_transactions.csv**: Sample dataset showing the flagged fraudulent transactions.

### Documentation
- **README.md**: This file, which provides an overview of the project, setup instructions, and usage.
- **architecture_diagram.png**: A high-level architecture diagram that illustrates the flow of data from Azure Data Lake to Synapse and Power BI.

## How to Use This Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/ecommerce-fraud-detection.git


  ### OUTPUT SCREENSHOTS
  ![image](https://github.com/user-attachments/assets/6d08ea96-b911-465a-8021-1d7ba6699d83)
  
  ### Fig[1]: Created a Resource Group
  
  ![image](https://github.com/user-attachments/assets/4d6eb4e1-7330-4cc8-806a-d88a67594612)
  
  ### Fig[2]: Then Created Data Lake Storage Account and created new containers to store our csv file 
  
  ![image](https://github.com/user-attachments/assets/7411c853-33ac-4541-b196-2587ec4a5f6c)
  
  ### Fig[3]:Then Created Synapse Workspace 
  
  ![image](https://github.com/user-attachments/assets/7f4907a7-193f-44f3-8edc-37c44996c314)
  
  ### Fig[4]:Then Open Synapse Analytics Workspace using Workspace web URL
  
  ![image](https://github.com/user-attachments/assets/7111c87b-7ad5-401a-9ae2-fa1352d334be)
  
  ### Fig[5]:Then Go to Data -> Linked -> Connect to our Data Lake here. Open New SQL Script + here -> Execute the SQL queries and save the SQL SCRIPT
  
  ![image](https://github.com/user-attachments/assets/120be28a-89fd-4452-adad-93efb04b1feb)
  
  ![Screenshot 2025-04-28 201129](https://github.com/user-attachments/assets/5511ae10-13d7-4ae0-aa87-fb713c108215)
  
  ![Screenshot 2025-04-28 202329](https://github.com/user-attachments/assets/4bc854e4-b7eb-4dc9-b1ce-3bbe0aa9a315)
  
  ### Fig[8]: Open Power BI Desktop -> Get Data -> Azure Synapse Analytics Workspace (Beta) -> connect
  
  ![Screenshot 2025-04-28 193249](https://github.com/user-attachments/assets/5d5ed8a9-39c2-4e50-9501-ee9695d1fe79)
  
  ### Fig[9]: Select the required columns and rows -> select the type of visualization -> To create Reports and Dashboards for analysis
  
  ![image](https://github.com/user-attachments/assets/2903693e-b023-47d6-87d4-5983b6ad5e70)
  
  ![image](https://github.com/user-attachments/assets/7d8507ec-5d67-4b81-bf54-090856c7d437)
  
  ### Fig[10]: Open the Azure Synapse workspace -> Manage -> Source Control -> Git Configuration -> Configure a repository -> GitHub account -> Repository Name / Link ->          collaboration branch -> Root folder -> save and commit for deployment 










