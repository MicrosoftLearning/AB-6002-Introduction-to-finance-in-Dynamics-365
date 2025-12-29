Module 5: Describe general ledgers and cash and bank management lab 1

# Lab: Create and view a journal

In this lab you will create, post, and view a journal in Dynamics 365 Finance. The purpose of a journal entry is to record a business transaction in an accounting book. You record journal entries in the ledger. You then use the ledger to create financial statements for the business.

Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Go to **General ledger \> Journal entries \> General journals.**
2.  Select **New** to create a new journal.
3.  Choose the journal name in the **Name** field on the newly created journal line.
4.  Select **Lines** to open the journal and add lines.
5.  On the first line, enter the **Account** field**.**
    -   Fill in the financial dimensions for the account and ensure the structure enforces correct dimension combinations (, if a business unit–department pair is invalid, a validation error appears).
6.  Enter the **Debit** amount.
7.  elect the **Offset account**.
8.  Select **Post** to post the journal. Highlight the functions to alidate or imulate posting prior to posting.
9.  ou want to search for the journal transaction(s) you just created.
10. Go to **General ledger \> Inquiries and reports \> Voucher transactions** o to **General ledger \> Inquiries and reports \> Accounting source explorer.**
11. Search for your posted transaction in either menu you choose from by the posted journal number.
12. Explore the transaction you posted and its voucher transactions.
    -   Select **Voucher** to view the posted vouchers for the transactions. This will open the **Voucher transactions** screen. View the line details of the transactions that you previously selected in the posted journal.
    -   **Voucher transactions** is an inquiry page where you can select from various tables and fields to specify criteria for the balance or transaction that you're searching for. By default, the page shows the journal number, voucher, date, and main account, but you can add additional tables, fields, and criteria to narrow down your search.
