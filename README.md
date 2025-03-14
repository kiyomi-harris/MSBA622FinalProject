# MSBA622FinalProject
## Overview

This project analyzes the financial records of the fake PSU Hotel to detect potential fraud using Malloy. The dataset includes journal entries from 2014 to 2016 and a 2016 trial balance. PSU Hotel's fiscal years are from July to June, so journal entries from 2014 are for the fiscal year 2015. There are only two fiscal years worth of transactions. The goal is to identify discrepancies, unusual transactions, and patterns indicative of fraudulent activity.

## Data Sources

je.csv: Contains journal entries from 2014–2016.

trailbalance.csv: Contains the 2016 trial balance with account balances.

Analytics_mindset_case_studies_PSU_Hotel_background.pdf: Background on PSU Hotel’s operations and financial context.

## Summary of Findings

### Transaction Summary

This chart showcases the different type and classes of accounts that PSU Hotel had transactions in. It shows that from 2015 to 2016 there was a large decrease in cash and a large increase in PPE. You can also see that the rest of the accounts stayed fairly similar from the two fiscal years, however the decrease in cash shows up in the fact that PSU Hotel has $1 million less in assets and their liabilites went from negative to positive.

![TransactionSummary](images/vis1.png)

### Transaction Entry Trend

This analysis visualizes credit and debit trends over time for different account types—Assets, Expenses, Liabilities, and Revenue—based on a general ledger dataset. The line charts display fluctuations in credits (left side) and debits (right side) from mid-2014 to mid-2016.

Assets & Revenue: Show significant negative credit values, suggesting outflows, while debits indicate ongoing inflows.
Expenses: Have relatively stable credit values, with a gradual increase in debits, implying rising costs.
Liabilities: Exhibit minimal fluctuations, suggesting steady financial obligations.

![EntryTrend](images/vis2.png)


## Who Prepares the entries?
This visualization provides an overview of transaction patterns by PreparerID, categorizing credits and debits across different account classes. While only a few preparers are visible, the full dataset includes more individuals handling financial transactions.

POS & GUESTSYS appear to be responsible for high-volume sales transactions, with large credits in "Sales - Other" and corresponding debits in "Cash."
Victoria Simpson (Accounting Manager) has a broader distribution of transactions, with debits spread across payroll, accounts payable, and other expenses, indicating involvement in financial operations beyond sales.

![preparerentries](images/vis3.png)

## Parts of the Hotel
The bar charts visualizes the financial data of the hotel’s general ledger for 2015 and 2016, displaying assets, liabilities, revenue, and expenses by hotel area. Each financial category is nested within the respective year, allowing for a clear comparison of amounts across different departments. This breakdown highlights trends and potential discrepancies in financial performance.

![busunit](images/vis4.png)

## Background and Motivation

Financial fraud can be difficult to detect, but data analytics offers a powerful way to uncover hidden anomalies. By leveraging tools like Malloy, this analysis provides insights into PSU Hotel’s financial health, highlighting unusual transactions and discrepancies that could indicate fraudulent activity. This report is valuable for auditors, financial analysts, and anyone interested in forensic accounting and fraud detection.

## Code

This repository contains two Malloy code files:

- [`final_sources.malloy`](final_sources.malloy), sources all the data tables for the data analysis portion of this repository.
- [`final2.malloynb`](final.malloynb), performs the analysis piece of the data provided by the Data Liberation Project.

## Why Malloy?
[Malloy](https://malloydata.dev) is an open source semantic data language, and a compelling alternative to pandas, ggplot, and SQL!


## How see the analysis yourself
Are you logged into github? Just press the period key right now. This will load the web editor. Then install the malloy extension. See images below for reference:
| **Step**   | **Image Preview** |
|--------|-----------|
| `Step 1 - Press allow` | <img src="images/step1.png" width="50%"> |
| `Step 2 - Click the Blocks, search for Malloy, install` | <img src="images/step2.png" width="50%"> |
| `Step 3 - Click Trust` | <img src="images/step3.png" width="50%"> |
| `Step 4 - Click a .malloynb file` | <img src="images/step4.png" width="50%"> |
| `Step 5 - Press Run` | <img src="images/step5.png" width="50%"> |


## Licensing

The files are provided directly from Earnst and Young Foundation. 
