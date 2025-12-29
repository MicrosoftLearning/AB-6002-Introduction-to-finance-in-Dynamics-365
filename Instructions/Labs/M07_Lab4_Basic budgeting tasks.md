---
lab:
    title: 'Lab 4: Basic budgeting tasks'
    module: 'Module 7: Describe expense management, fixed asset management, and budgeting'
---

# Module 7: Describe expense management, fixed asset management, and budgeting

## Lab 4: Basic budgeting tasks

## Objectives

In this lab, you will create budget register entries and approve them. Then you will run the budget-to-actuals report. We will work with January 2018 in legal entity USMF because it contains “actuals” data in this period to compare to our budget entries.

## Lab Setup

- **Estimated Time**: 20 minutes

## Tasks

1.  In the **Navigation** pane, select **Modules** \> **Budgeting** \> **Budget register entries**.
2.  Select **New** in the Action pane.
3.  Select **FY2018** in the **Budget model** drop-down list.
4.  Select **Original budget** in the **Budget code** drop-down list.
5.  Select the **Add line** menu item in the **Budget account entries** FastTab.
6.  Add the following entries.

| Date     | Account structure | Dimension values            | Amount    | Amount type | Currency | Comment                                          |
|----------|-------------------|-----------------------------|-----------|-------------|----------|--------------------------------------------------|
| 1/1/2018 | Manufacturing B/S | 140100-002-023              | 1,000.00  |             | USD      | Onhand inventory for production at start of year |
| 1/1/2018 | Manufacturing B/S | 140200-002-023              | 5,000.00  |             | USD      | Onhand finished goods at start of year           |
| 1/1/2018 | Manufacturing P/L | 401100-001-023-010-TV&Video | 40,000.00 | Revenue     | USD      | TV Sales                                         |
| 1/1/2018 | Manufacturing P/L | 601200-001-023-010-TV&Video | 5,000.00  | Expense     | USD      |                                                  |
| 1/1/2018 | Manufacturing P/L | 500100-001-023-010-TV&Video | 10,500.00 | Expense     | USD      |                                                  |

1.  Select **Update budget balances** in the Action pane at the top of the page. Leave the defaults and select OK. An **Operation completed** message should appear. These budget entries are no longer in draft mode and are considered your January 2018 budget. Notice how the status is changed to **Completed** in the upper right of the page.
2.  In the **Navigation** pane, select **Modules** \> **Budgeting** \> **Inquiries and reports** \> **Basic budgeting** \> **Actual vs. budget**.
3.  Select **MA+BU+DEPT+CC** for the **Financial dimension set**.
4.  Select **FY2018** as the **Budget model.**
5.  Select **1/1/2018** as the **Start date** and **1/31/18** as the **End date**.
6.  Leave other fields with default values and select **Apply parameters** in the Action pane.
7.  Review the report. Notice that two accounts had actuals for which you did not enter budget lines. The budget column is zero for those accounts. The accounts you entered budget in are showing in the Budget column with the amounts you entered.

# Summary

When a full budget for the year is entered, it includes values for each period in the fiscal year. Throughout the year, the budget-to-actuals report can be run to examine how closely the actuals match the budget. When they don’t match, you should either update the budget or adjust the actuals by lowering expenses or raising revenue. The budget-to-actuals report provides a high-level view to begin the analysis of the variance. Creating a budget and periodically running the budget-to-actuals report helps a company stay on track throughout the fiscal year, adjusting budget numbers or processes so the budget and actuals align with expectations.

# Reference screenshots

![](media/445f541e8165ecfddd1f790cb8e2b4e2.png)

![](media/5a2583bfa6060be2e5bee0085e16c5c1.png)

![](media/fa0bc3673134ac3b6131f5a7b18293ae.png)

![](media/646ed85c833b122b200fbc7381bdd750.png)

![](media/431a6f948fef07027601ef14388cf8df.png)

![](media/384ff5c2808c13b8de46ed662573bf90.png)

![](media/73abe92b14b69ace03abcb611a37007f.png)

