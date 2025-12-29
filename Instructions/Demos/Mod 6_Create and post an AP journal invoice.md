Module 6: Describe accounts payables, accounts receivables, and credit and collections 

# Demo: Create and post an AP invoice journal

In this demo, we explore the process of creating, posting, and viewing an AP invoice journal in Dynamics 365 Finance. Creating and posting an AP invoice journal records an expense and establishes a liability to the vendor. This process updates the general ledger and vendor account, ensuring accurate financial reporting and payment tracking.

Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Go to **Accounts payable** \> **Invoices** \> **Invoice journal**.
2.  Select **New** to create a new journal.
3.  Choose the journal name in the **Name** field on the newly created journal line; for this example, select **APInvoice**.
    -   Explain that journal names are set up for different types of journals, and this example is a general journal. Briefly explain that different journal names determine which types of postings are allowed.
4.  Select **Lines** to open the journal and add lines.
5.  On the first line, enter the vendor **Account**. Choose **1001 Acme Office Supplies**. The Account type is automatically populated with Vendor since this is a vendor invoice journal. Explain how all the accounts and dimensions will display in the drop-down menu for selection.
    -   For this demo, we will **NOT** manually enter financial dimensions for the vendor line. Instead, we want to show how they automatically flow from the vendor defaults and main account setup.
6.  Show the Financial dimensions for the account. Choose **Financial dimensions** \> **Account** in the tab above the lines. Explain that this automatically flows and fills in the financial dimensions for the account based on the saved default financial dimensions from the vendor.
7.  Enter the **Invoice date** and **Invoice**. These would be provided by the vendor. (For the demo example, use any past date and any test invoice number, such as *123AcmeInvoice*).
8.  In the **Credit** field, enter an amount, such as \$1000.00, the amount of the vendor invoice.
9.  Select the **Offset account** and select an expense account number, *606300 Office Supplies Expense*. Highlight that the financial dimensions automatically populated correctly based on the defaults set for that account. Note that the dimensions on the expense line came from the main account posting profile, while the vendor line inherited dimensions from the vendor default dimensions.
    -   Explain that the **Sales tax group** defaults from the vendor account, and the **Item sales tax group** defaults from the main account that's specified in the **Offset account** field. Additionally, the system calculates the due date based on the terms of payment, and then the cash discount defaults from the vendor account.
10. Select **Post** to post the journal. Highlight the functions to **Validate** or **Simulate posting** prior to posting that assists with validating the journal before posting.
    -   After posting, open **Voucher transactions** quickly to show and confirm that both sides of the journal reflect the expected financial dimensions from their respective sources.
