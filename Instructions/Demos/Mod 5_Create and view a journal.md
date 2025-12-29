Module 5: Describe general ledgers and cash and bank management demo 1

# Demo: Create and view a journal

In this demo, we want to show the process of creating, posting, and viewing a journal in Dynamics 365 Finance. The purpose of a journal entry is to record a business transaction in an accounting book. You record journal entries in the ledger. You then use the ledger to create financial statements for the business.

Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Go to **General ledger \> Journal entries \> General journals.**
2.  Select **New** to create a new journal.
3.  Choose the journal name in the **Name** field on the newly created journal line; for this example, select **GenJrn**.
    -   Explain that journal names are set up for different types of journals, and this example is a general journal. Briefly explain that different journal names determine which types of postings are allowed. With this journal, you can post financial transactions to general ledger accounts and other accounts, such as bank, customer, and vendor accounts.
4.  Select **Lines** to open the journal and add lines.
5.  On the first line, enter the **Account**. Explain how all the accounts and dimensions will display in the menu for selection. Choose account **600250 Salaries Manufacturing**. Then select the following dimensions:
    -   **Business unit:** 001 Home
    -   **Department:** 026 Human resources
    -   **Cost center:** 010 Production
    -   **Item group:** Leave blank

        Explain that this fills in the financial dimensions for the account and that the structure enforces correct dimension combinations (for example, if a business unit–department pair is invalid, a validation error appears). This helps maintain data integrity and consistent reporting.

6.  Enter the **Debit** amount, **1000.00**.
7.  Select the **Offset account**. Select **110160**, the payroll account. Highlight that the financial dimensions automatically populated correctly based on the defaults set for that account.
8.  Select **Post** to post the journal. Highlight the functions to validate or simulate posting before posting.
9.  Select **Voucher** to view the posted vouchers for the transactions. This will open the **Voucher transactions** screen. Highlight the line details of the transactions that you previously selected in the posted journal.
    -   **Voucher transactions** is an inquiry page where you can select from various tables and fields to specify criteria for the balance or transaction that you're searching for. By default, the page shows the journal number, voucher, date, and main account, but you can add additional tables, fields, and criteria to narrow down your search.
10. While still on the **Voucher transactions** screen, select **Accounting source explorer**.
    -   View the posted voucher and briefly highlight that this page can be used for detailed analysis of the source information behind general ledger accounting entries.
