# Business-Aware Prompt Design for Text-to-SQL in E-Commerce Analytics

This repository contains the code, experimental configurations, and evaluation resources for our study on **business-aware prompting for Text-to-SQL in e-commerce analytics**.

The proposed approach enriches LLM prompts with three types of business context: **enhanced schema descriptions, KPI definitions, and business rules**, aiming to improve the semantic correctness of generated SQL queries for business analytics.

The implementation uses **GPT-4o-mini**, **PostgreSQL via Supabase**, and the **Brazilian E-Commerce Public Dataset by Olist**.

## 1. General Overview

This project implements a business-aware Text-to-SQL pipeline that translates Vietnamese natural-language business questions into executable SQL queries.

The source code is implemented in Google Colab, while Supabase is used to host the PostgreSQL database.

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

## 5. How to cite
If you find this work, code, or evaluation resources useful, please cite our paper:

Huynh-Ngan La, Hoang T. Nguyen, and Hung-Nghiep Tran
[BAPTSQL: Business-Aware Prompt Design for Text-to-SQL in E-Commerce AnalyticsL](https://github.com/lahuynhngan/BAPTSQL). CONF XXX, 2026. doi:10.1234/abcxyz
