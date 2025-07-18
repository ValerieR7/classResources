Superstore Customer Analysis: Comprehensive Prompt Workflow
This document outlines a detailed, structured workflow of prompts for conducting a customer behavior analysis on the Superstore dataset. It includes initial context-setting and best-practice prompts for a more effective and realistic analytical process using an AI assistant.

0. Environment & Persona Setup
This foundational set of prompts establishes the AI's role and the context of the project, which is a critical first step for guiding the model's responses.

Prompt 0.1: Set AI Persona

"You are an expert data analyst and business strategist. Your goal is to help me perform a customer behavior analysis using the DIVE framework. You will provide expert guidance, generate code, and help interpret the results to derive actionable business strategies."

Prompt 0.2: Define Project Context & Tools

"I am working in a Google Colab notebook connected to BigQuery. My dataset is a table named superstore_dataset. All SQL queries you generate must be compatible with BigQuery syntax, and all Python code should be suitable for a Colab environment, primarily using libraries like Pandas, Matplotlib, and Seaborn."

1. Setup & Initial Exploration (EDA)
This phase focuses on understanding the dataset's structure and ensuring data quality before analysis.

Prompt 1.1: Define Business Questions

"As a customer behavior strategist analyzing the superstore_dataset, identify the top 5 business questions to investigate. Focus on themes like customer value, purchasing patterns, and retention."

Prompt 1.2: Explain Question Importance

"For each of the 5 business questions, explain its business importance and list the specific data columns required for the analysis."

Prompt 2.1: Generate Descriptive Statistics

"Generate a descriptive statistics summary for the superstore_dataset to support a customer behavior analysis."

Prompt 2.2: Identify Data Quality Issues

"Based on the descriptive statistics, identify potential data quality issues that could affect the analysis. For each issue, explain what statistical patterns might indicate a problem."

Prompt 2.3: Suggest Validation Queries

"Suggest specific BigQuery validation queries to investigate the identified data quality issues."

Prompt 3.1: Generate Validation Code

"Generate the Python and BigQuery code needed to run the validation queries. The code should identify and display records with potential data quality issues, such as zero sales with positive quantity or shipping dates that occur before order dates."

Prompt 3.2: Explain Validation Code

"Please add comments to the code you just generated, explaining what each section does."

2. DIVE Framework: Discovery Phase
This phase focuses on customer segmentation using the RFPM (Recency, Frequency, Profit, Monetary) model.

Prompt 4: Calculate RFPM Values

"Begin the Discovery phase of the DIVE framework. Generate a BigQuery query to calculate Recency, Frequency, Profit, and Monetary (RFPM) values for each customer in the superstore_dataset."

Prompt 5.1: Rank Customers into Quintiles

"Using the calculated RFPM values, generate a query to rank each customer into quintiles (from 1 to 5) for each of the Recency, Frequency, Profit, and Monetary dimensions."

Prompt 5.2: Segment Customers

"Now, using the RFPM quintile scores, write a query to classify each customer into predefined segments. Use the following segmentation logic: Champions (R=5, F=5, P=5), Loyal Customers (R=3-4, F=4-5, P=4-5), Promising/New (R=5, F=1-2, P=1-2), At-Risk Customers (R=1-2, F=4-5, P=4-5), and Lost Customers (R=1, F=1, P=1)."

Prompt 6.1: Visualize Revenue Trends

"Generate Python code to create a line chart visualizing customer revenue and average order value trends over time."

Prompt 6.1a: Interpret Revenue Trends

"Based on the chart you just created, what are the key takeaways from the revenue and AOV trends?"

Prompt 6.2: Visualize Regional Sales

"Generate Python code to create a map or bar chart showing the concentration of customer sales by region."

Prompt 6.2a: Interpret Regional Sales

"What insights can we gather from the regional sales visualization?"

Prompt 6.3: Visualize Customer Retention

"Generate Python code for a pie or bar chart that displays the proportion of repeat customers versus one-time customers."

Prompt 6.3a: Interpret Customer Retention

"What does this retention chart tell us about our customer base?"

3. DIVE Framework: Investigate Phase
This phase delves deeper into understanding the behaviors that differentiate key customer segments.

Prompt 7.1: Compare Product Preferences of High-Value Segments

"Begin the Investigate phase. To understand what differentiates our high-value segments, first compare the product preferences of 'Champions' versus 'At-Risk' customers. Does one group purchase more profitable products?"

Prompt 7.2: Analyze Discount Impact on Champions

"Next, analyze the impact of discounts on the profitability of the 'Champions' segment. Determine if their high value is driven by full-price purchases or if they are also sensitive to discounts."

Prompt 8: Conduct Market Basket Analysis

"Perform a market basket analysis on the 'Champions' segment. Generate a query to identify the top 10 most frequently co-purchased product sub-category pairs for these customers."

4. DIVE Framework: Validate & Extend Phase
This final set of prompts focuses on validating hypotheses and extending the analysis to generate actionable business strategies.

Prompt 9: Test Geographic Churn Hypothesis

"Begin the Validate phase. Test the hypothesis that customer churn is localized by generating a visualization that compares the geographic distribution (by state) of 'Champions' and 'At-Risk High-Value' customers."

Prompt 10: Quantify Profit at Risk

"To quantify the financial impact of churn in specific locations, calculate the total historical profit from 'At-Risk High-Value' customers, broken down by state."

Prompt 11: Propose 'Toxic Market' Strategy

"Now, enter the Extend phase. Based on the finding that states like Ohio and Pennsylvania are unprofitable 'toxic markets' with high churn, propose a 'Market Health Review and Intervention' strategy. The proposal must define the business problem, target market, specific actions, and a measurable financial goal."

Prompt 12: Propose High-Value Customer Strategy

"Based on the analysis of 'Champions' and 'At-Risk High-Value' segments, propose a dual strategy. First, design a 'White Glove' retention program for 'Champions'. Second, create a 'Proactive Win-Back' campaign for 'At-Risk High-Value' customers. For each strategy, define the target, action, and financial goal."

AI Usage Log
AI Tool Used: Gemini

Primary Role: The AI acted as an expert analytical partner.

Key Interactions:

Context & Persona Setting: Established the AI's role and the technical environment for the project.

Code Generation: Generated SQL queries for BigQuery and Python code for data manipulation and visualization.

Code Explanation: Provided comments and explanations for generated code to ensure clarity.

Data Quality Assessment: Assisted in identifying potential data quality issues and suggesting validation steps.

Analysis & Interpretation: Provided summaries and interpretations of analytical outputs, such as charts and tables.

Strategy Formulation: Brainstormed and structured actionable business strategies based on the analytical findings.