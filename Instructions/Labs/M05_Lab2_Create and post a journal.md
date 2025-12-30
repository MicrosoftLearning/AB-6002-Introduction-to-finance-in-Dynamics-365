---
lab:
    title: 'Lab 2: Create and post a journal'
    module: 'Module 5: Describe general ledgers and cash and bank management'
---

# Module 5: Describe general ledgers and cash and bank management

## Lab 2: Create and post a journal

## Objectives

In this lab you will create, post, and view a journal in Dynamics 365 Finance. The purpose of a journal entry is to record a business transaction in an accounting book. You record journal entries in the ledger. You then use the ledger to create financial statements for the business.

## Lab Setup

- **Estimated Time**: 10 minutes

## Tasks
Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Go to **General ledger \> Journal entries \> General journals.**
2.  Select **New** to create a new journal.
3.  Choose **General journal** in the **Name** field on the newly created journal line.
4.  Select **Lines** to open the journal and add lines.
5.  On the first line, select **Account** field **110110**, **BusinessUnit** field **001**, and **Department** **023**.
6.  Enter a **Debit** amount of 100.
7.  Select the **Offset account** **401200**.
8.  Select **Post** to post the journal. 
9.  You want to search for the journal transaction(s) you just created.
10. Go to **General ledger \> Inquiries and reports \> Voucher transactions** or go to **General ledger \> Inquiries and reports \> Accounting source explorer.**
11. Search for your posted transaction in either menu you choose from by the posted journal number.
12. Explore the transaction you posted and its voucher transactions.
    -   Select **Voucher** to view the posted vouchers for the transactions. This will open the **Voucher transactions** screen. View the line details of the transactions that you previously selected in the posted journal.
    -   **Voucher transactions** is an inquiry page where you can select from various tables and fields to specify criteria for the balance or transaction that you're searching for. By default, the page shows the journal number, voucher, date, and main account, but you can add additional tables, fields, and criteria to narrow down your search.



