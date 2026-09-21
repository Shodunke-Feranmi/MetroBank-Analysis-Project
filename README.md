# MetroBank Analytics Challenge

An end-to-end, five-stage analysis of a retail bank's data, moving from **who the customers are** to **what they do**, **how they bank**, **how branches perform**, and **where service and fraud risk sit**.

---

## 📌 Project Overview

MetroBank is a fictional retail bank with Retail, Corporate, and Private customers. Across five stages I played different analyst roles (marketing, relationship management, operations, branch strategy, and customer experience/risk) to answer the questions each business function would realistically ask.

The project uses five connected datasets:

| Dataset | Grain | Used in |
|---|---|---|
| `Customers.csv` | One row per customer | Weeks 1, 2, 3, 5 |
| `Accounts.csv` | One row per account | Weeks 2, 3, 5 |
| `Transactions.csv` | One row per transaction | Week 3 |
| `Branches.csv` | One row per branch | Week 4 |
| `Complaints.csv` | One row per complaint | Week 5 |

## 🎯 Business Problem

A bank makes decisions with incomplete pictures: marketing doesn't know its customer mix, relationship managers don't know which products customers actually hold, operations doesn't know which channels carry the value, executives don't know which branches earn their cost, and risk teams don't know how quickly fraud cases are being handled.

This project pulls those views together into one connected picture of the bank.

## 📊 Project Objectives

- Profile and segment the customer base by demographics, income, and loyalty
- Measure product penetration, deposit strength, credit quality, and loan exposure
- Understand transaction behavior by type, channel, and merchant
- Evaluate branch profitability, efficiency, and cost control to guide investment
- Diagnose complaint drivers and flag high-risk fraud cases for urgent action
- Translate every analysis into clear findings for non-technical decision-makers

## 🗂️ Project Structure

```
├── Week 1 - Customer Profiling & Segmentation
├── Week 2 - Accounts, Balances & Credit
├── Week 3 - Transaction Behavior & Patterns
├── Week 4 - Branch Performance & Efficiency
└── Week 5 - Customer Experience & Risk Intelligence
```

Each folder contains the Excel workbook and, where applicable, the PowerPoint summary for that stage.

## 🛠️ Tools & Technologies

- **Microsoft Excel**: data cleaning, calculated columns (`IF`, `IFS`, `DATEDIF`, `TODAY`), lookups to link datasets, PivotTables, Pivot Charts, Slicers, Timelines, dashboards
- **Microsoft PowerPoint**: executive-facing summaries of findings

<!-- Only add SQL, Power Query, or Power BI here if you actually used them. -->

## 📈 Analysis & Key Findings

### Week 1: Customer Profiling & Segmentation
**Question:** Who is the MetroBank customer?
**Dataset:** `Customers.csv`

Built age-group (Gen Z, Millennial, Gen X, Boomer) and income-bracket (Low, Medium, High, Premium) segments, calculated customer tenure, and summarized the base by region, gender, and customer type in a one-page dashboard.

**Findings:**
- Total customers: We have 500 Customers
- Regional and gender split: We have 244 male nad 256 male customers, There are 110 customers in west, 120 in the North, 137 in the south, 133 in the East
- Largest age group / income bracket: Millennials is the largest Age group and High Income as the largest income bracket
- Largest customer segment: Retail is the largest Customer Segment with 286 customers  | Highest average income: Private customers have the highest average income with $118,774

### Week 2: Accounts, Balances & Credit
**Question:** What do customers actually use, and how healthy is the portfolio?
**Datasets:** `Accounts.csv` linked to `Customers.csv`

Analyzed product mix (Checking, Savings, Credit Card, Loan), multi-product customers, total deposits, the approved loan book, and the relationship between credit score and loan approval.

**Findings:**
- Account type distribution: From my analysis we have 303 Savings account, 246 Checking, 169 Creditcard and 82 Loan Accounts
- Total Balance: $145,013,181  | Approved loan Amount: The total approved loan amount is $3,677,399
- Average credit score, and approved vs. rejected gap: MetroBank Account has an average Credit score of 580 which is a Fair Credit score
- Highest average balance by segment; Boomers vs. Gen Z: Gen z have a higher average balance than the Boomers

### Week 3: Transaction Behavior & Patterns
**Question:** How do customers use their accounts?
**Datasets:** `Transactions.csv` linked to `Accounts.csv` and `Customers.csv`

Enriched the transaction data with account type and customer segment, then analyzed volume and value by type, channel, and merchant. Grouped dates by month to spot trends, and built an interactive dashboard with slicers and timelines.

**Findings:**
- Total transactions / total value / average amount: MetroBank has a total of 5000 Transaction having a average transaction amount of $5,013 and total transaction value of $25,066,089
- Breakdown by transaction type: Our Customers use all four of our transaction type well with withdrawal and payment type Transaction both having 1266 number of transaction each and Deposit having 1244 transactions and Deposit 1224 but the Withdrawal has the Highest transaction amount while Transafer has the least. 
- Most popular channel vs. channel carrying the highest-value transactions: THe most popular Transaction channel is POS having 1286 transactions and still having the highest Transaction amount

### Week 4: Branch Performance & Efficiency
**Question:** Where should the bank invest, and where should it streamline?
**Dataset:** `Branches.csv`

Evaluated branches on profitability, efficiency (revenue per staff member), and cost management to support an investment decision.

**Findings:**
- Most and least profitable branches: The south has been our most fitable Branch so far and East the least Profitable
- Cost management concerns: Javiertown has the highest Operating cost 

### Week 5: Customer Experience & Risk Intelligence
**Question:** What is driving complaints, and which fraud cases need action now?
**Datasets:** `Complaints.csv` linked to `Customers.csv` and `Accounts.csv`

Analyzed complaint types and trends, resolution times, and the open backlog. Then correlated complaints with segment, region, product, and account balance. Finally built a priority-flag system for high-risk fraud cases (for example, open fraud cases older than 7 days).

**Findings:**
- Most common complaint type and overall trend: Charges Dispute is the most common complaint Type 
- Average resolution time; slowest complaint type: The average solution time is 31 days and others has the slowest solution time
- Open / in-progress backlog and its age: We still have 157 Opened and 172 In progress cases 
- Are high-balance customers complaining more? Yes most Cmplaints are comng from our High value customers
- Active fraud cases / total ever reported / cases flagged as urgent: We still have 54 active active Fraud  cases, 145 fraud cases has bee reprted so far.

## 💡 Business Insights

Write 3 to 5 conclusions that cut across the weeks, for example:

1.  From the Customer analysis I would do a campaign targeting for the Gen Z age group beacuse they are the least age groups customers
2.  (e.g., where deposit or credit risk is concentrated)
3. `[ ]` (e.g., which channels to invest in based on transaction value)
4. `[ ]` (e.g., which branches to invest in or review)
5. `[ ]` (e.g., what the complaint and fraud backlog means for retention and risk)

## 📸 Dashboard / Visualizations

![Week 1 Customer Profile Dashboard](https://github.com/Shodunke-Feranmi/MetroBank-Analysis-Project/blob/main/Metrobank%20customers%20Dashboard.png)
![Week 2 Accounts & Credit]())
![Week 3 Transactions Dashboard]([images/week3_dashboard.png](https://github.com/Shodunke-Feranmi/MetroBank-Analysis-Project/blob/main/MetroBank%20Transaction%20Dashboard.png))
![Week 4 Branch Performance]([images/week4_summary.png](https://github.com/Shodunke-Feranmi/MetroBank-Analysis-Project/blob/main/MetroBank%20Branch%20Performance%20Dashboard.png))
![Week 5 Complaints & Fraud]([images/week5_summary.png](https://github.com/Shodunke-Feranmi/MetroBank-Analysis-Project/blob/main/MetroBank%20Complaints%20Dashboard.png))

## 📚 Skills Demonstrated

- Data cleaning and preparation
- Feature engineering with calculated columns (`IF`, `IFS`, `DATEDIF`)
- Linking multi-table datasets to build a connected analysis
- PivotTables, grouping, Pivot Charts, Slicers, and Timelines
- Dashboard design
- Customer segmentation and profitability analysis
- Credit, transaction, and complaint/fraud analysis
- Building a priority-flag system for risk triage
- Communicating findings to executive, non-technical audiences

## 👤 Author
Shodunke Feranmi
[GitHub](https://github.com/your-username)

