

#  Fetch Rewards – Data Analyst Take-Home Assessment
 
This repository contains my submission for the **Fetch Data Analyst Take-Home Exercise**. My goal in this project was not just to answer the questions, but to demonstrate how I approach ambiguous datasets, ensure data quality, and clearly communicate findings to both technical and non-technical audiences.

---

This repo is organized into three parts, based on the assessment's structure:

1. **Data Exploration & Quality Review**  
2. **SQL Queries: Insights & Assumptions**  
3. **Stakeholder Communication**

Each section includes detailed commentary, code (with context), and a clear trail of thought behind the analysis. I’ve worked to make it easy to follow even if you’re unfamiliar with the raw dataset.

---

## Part 1: Data Exploration & Quality Review

In this section, I took the time to understand the structure, cleanliness, and quirks of the data. Rather than jump straight into queries, I believe it's critical to first ensure we're working with reliable inputs.

**Key issues I uncovered:**

- **Incomplete or inconsistent data**: Missing values in several key columns.
- **Duplicate records**: Present in both Transactions and Products datasets; could lead to inflated counts if not handled properly.
- **Logical inconsistencies**: One user account had a creation date *before* their birthdate, which isn't feasible.
- **Formatting issues**:
  - Brand/store names with typos 
  - Inconsistent gender labels (two versions of "non-binary")
  - Birthdates in multiple formats
- **Confusing timestamp order**: Some purchase dates came after scan dates, which raised red flags.
- **Mixed data types in quantity field**: Numbers and letters were used interchangeably in the same column, affecting numerical analysis.

Rather than ignore these, I documented each issue and how it might impact results.

---

## Part 2: SQL-Based Analysis

For this section, I chose a mix of closed and open-ended questions. You’ll find the respective query for each question, along with the assumptions made when necessary.

**Closed-ended questions:**  
> Top 5 brands by receipts scanned among users aged 21 and over
> Top 5 brands by sales among users who have had their account for 6 months or more


**Open-ended example:**  
> What is the leading brand in the Dips & Salsa category?

**Interesting Insight:**  
The same top brands showed up for two seemingly different user groups (users over 21 vs. users with accounts older than 6 months). After investigating, I found these groups overlapped entirely—highlighting the importance of checking assumptions before jumping to conclusions.

---

## Part 3: Communicating with Stakeholders

Data is only valuable when it's communicated well.

I included a business-facing summary (Slack/email-style) written in plain language, without technical jargon. It outlines:
- Key data issues
- One trend worth investigating further
- Follow-up questions that could help us make sense of confusing patterns

I approached this message as I would in a real business setting, tailoring to someone without a data background.

---

##  Tools Used

- SQL (PostgreSQL)
- Python (for EDA and validation)
- Pandas, Seaborn, Matplotlib (for light visualizations)

---

Thank you for reviewing my submission. I hope it gives you a sense of how I work. If you'd like to walk through any part of this in more detail, I'd be happy to chat!

Warm regards,  
**Prashanti**  
