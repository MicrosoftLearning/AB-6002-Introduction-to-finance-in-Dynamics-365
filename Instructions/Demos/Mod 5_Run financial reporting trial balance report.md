Module 5: Describe general ledgers and cash and bank management demo 2

# Demo: Run Financial reporting trial balance report

In this demo, we want to show the process of running a trial balance report by using Financial reporting in Dynamics 365 Finance. We will show the voucher posting from the previous demo.

Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Go to **General ledger \> Inquiries and reports \> Financial reports**.
    -   Explain that **Financial Reporter** uses the shared data from the general ledger to build formatted financial statements like balance sheets, income statements, and trial balances.
    -   Mention that reports can be customized or scheduled for recurring use.
2.  Highlight the default report definitions available in the Financial reports and select **Summary Trial Balance – Default** from the list of reports.
    -   Briefly explain that several versions of trial balance reports are available:
        -   **Summary Trial Balance** shows summarized debit and credit totals by main account.
        -   **Detailed Trial Balance** provides transaction-level detail, which is useful for auditors or controllers.
        -   **Detailed JE and TB Review** combines journal entry details with trial balance for deeper analysis.
3.  Select **Generate**. When prompted, select the current period or the period in which you posted your journal (should be today’s date for the demo example).
    -   Explain that this report pulls data directly from posted vouchers, ensuring accuracy and real-time reflection of financial data.
4.  The financial report will be generated while you continue to work. While the report generates, explain that the **Reports** view on the screen will contain the previously generated reports that can be viewed until the expiration date. Refresh the screen to view the generated report.
5.  Select the report date in the list and view the report output.
    -   When the report opens, locate the ledger account used in the demo, “Describe general ledgers and cash and bank management” (**600250 – Salaries Manufacturing**).
    -   Highlight that the debit amount of **1,000.00** appears in the report.
6.  Drill down to the transaction level.
    -   Select the account line and drill down to the voucher transactions. Show the voucher created in the demo, “Describe general ledgers and cash and bank management.”
    -   Emphasize how users can navigate seamlessly from summarized financial data to the detailed voucher for transparency and audit purposes. Highlight the additional features of the report including **Report options** to filter, print, and export.
7.  Close the report and summarize that Financial Reporter provides flexible, real-time visibility into ledger balances.
