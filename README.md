## 1. General Overview
This pipeline builds an automated business data analysis chatbot from natural language—supporting Business Development in analyzing business performance. 
The source code is written entirely on Google Colab and uses Supabase as the database.

## 2. Directory Structure
- `Group1_Notebook.ipynb`: Main source code file (Google Colab Notebook) containing the entire pipeline.
- `database_schema.sql`: Table structure and functions/triggers (if any) used in Supabase.
- `data` folder: Data extracted from Supabase to ensure reproducibility.
- `README.md`: Installation and setup instructions.

## 3. Execution Instructions

To run this project, please follow these steps:

**Step 1: Environment Setup**
1. Open Google Colab.
2. Upload the `Group1_Notebook.ipynb` file to Google Colab.

**Step 2: Database Setup**
- Go to the SQL Editor in Supabase and run the content in `database_schema.sql` to create tables.
- Extract the `data` folder.
- Upload each file in the `data` folder into the newly created tables to populate the test data.

**Step 3: Key / URL Configuration**
This project requires connection to Supabase and the gpt-4o-mini API. 
Please navigate to the 'Load data' cell and the 'Set-up API Key' cell.
- `SUPABASE_URL`: [Enter your Supabase URL]
- `OPENAI_API_KEY`: [Enter your API Key]

**Step 4: Run the Pipeline**
- Run each cell sequentially from top to bottom in the Notebook.
- Observe and evaluate the results.

## 4. Dataset
- Database name: Brazilian E-Commerce Public Dataset by Olist
- Link: kaggle.com/datasets/olistbr/brazilian-ecommerce
