Module 6: Describe accounts payables, accounts receivables, and credit and collections lab 1

# Lab: Create and pay an account payables invoice

In this lab, you’ll create and post an accounts payable invoice journal. Then you’ll create a vendor payment for the invoice in Dynamics 365 Finance.

Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Go to **Accounts payable** \> **Invoices** \> **Invoice journal**.
2.  Select **New** to create a new journal.
3.  Choose the journal name in the **Name** field on the newly created journal line and choose **APInvoice**.
4.  Select **Lines** to open the journal and add lines.
5.  On the first line, enter the vendor **Account** (example US-103 Rain Projectors).
6.  Enter the **Invoice date** and **Invoice**. These would be provided by the vendor (for the lab example, use any past date and any test invoice number, such as *123AcmeInvoice*).
7.  Enter the **Credit** amount, which would be the amount of the vendor invoice.
8.  Next, select the **Offset account**. Select an expense account number, *606300 Office Supplies Expense*. The financial dimensions automatically populate correctly based on the defaults set for that account.
    -   Note that the dimensions on the expense line came from the **main account posting profile**, while the vendor line inherited dimensions from the **vendor default dimensions**.
9.  Select **Post** to post the journal.
10. Next, you want to pay the vendor invoice that was just posted. Go to **Accounts payable** \> **Payments** \> **Vendor payment journal**.
11. Select **New** to create a new journal.
12. Choose the journal name in the **Name** field on the newly created journal line and choose **VendPay.**
13. Select **Lines** to open the journal and add lines.
14. In the journal, select **Payment proposal** \> **Create payment proposal**. You will select the invoice that was previously posted to pay in the next steps.
15. Select the **Minimum payment date** as 30 days from today’s date to capture the invoice previously posted for payment.
16. Enter other query restrictions under **Records to include**. Filter by the vendor for payment (vendor US -103).
17. Select **OK**. After you select OK, the results of the query appear.
18. Select the invoices for payment. Remove any unwanted payment lines by selecting **Remove** before selecting **Create payments**. The invoice created in the previous step should be selected. If other invoices are selected, those will also be included in the payment journal.
19. Select **Create payments**. The **Create payments** button creates vendor payments in the payment journal.
20. The payment lines are created and marked for settlement against the invoices from the payment proposal.
21. Select the **Method of payment** for the line as type **ELECTRONIC** to post the journal without generating payments or checks for this example.
22. Post the journal.
23. Navigate to **Accounts payable** \> **Vendors** \> **All vendors**. Filter and select the vendor from the previous transaction. Select **Balance** in the Action bar under **Vendor** \> **Transactions** to view the vendor balance. Note the current vendor balance.
24. From the vendor balance, select **Open transactions** to view the open vendor transactions. Select **Closed transactions** to view closed transactions, which will include paid invoices.
25. Lastly, select **Settlement** \> **Undo settlement** in the same screen to view the settled transactions. The settlement from the posted vendor payment will be displayed. This settlement was automatically settled by creating the payment proposal with the marked vendor invoice.
