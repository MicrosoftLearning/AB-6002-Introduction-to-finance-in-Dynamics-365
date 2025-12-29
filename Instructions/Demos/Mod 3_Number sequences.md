Module 3: Demo – Number sequences

Number sequences allow the system to create unique recognizable numbers for records in finance and operations apps without user intervention. Some examples of the types of sequences used include:

-   Customer and vendor IDs
-   Journal batch numbers
-   Voucher numbers
-   Vendor invoice numbers

In this demo, we review number sequences. We discuss:

-   Defining the format
-   Additional options
-   Specifying references and where it’s used

Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.

1.  Navigate to **Organization administration** \> **Number sequences** \> **Number sequences**.
2.  Use the quick filter to find number sequence **Gene_113**. Select the **number sequence code** hyperlink to open the details page.
3.  Select **Edit** in the menu bar at the top of the form.
4.  Display the Scope drop-down menu. Explain that the two most often used scopes are **Shared** and **Company**. *Shared* is for global data. *Company* is for company specific. Reference Learn to get information about the other options.
5.  Next, focus on the **Segments** FastTab. Select **Add** to display a line where you can show the options available for a segment.
    -   **Alphanumeric**: Generated number.
    -   **Constant**: A value that appears in every generated number. Generally, this is used in sequences to distinguish one entry type from another.
    -   **Company**: Legal entity and company ID. Often the company ID is used as a prefix in multi-company organizations.

        The value generated from this sequence is all numeric; no company prefix or constant value are included.

6.  Select **Remove** because you need to leave the sequence unchanged.
7.  Expand the **References** FastTab. When a reference is listed, that generally means you’ll find this number sequence specified on the **Number sequence** tab of a parameters form. Duplicate this tab and navigate to **General ledger** \> **Ledger setup** \> **General ledger parameters**. Select the **Number sequences** tab. This is the first one listed, the **Journal batch number**. Every journal in the system has a batch number; those numbers all use this sequence.
8.  Go back to the **Number sequence details** page and expand the **General** FastTab. Describe the following:
    -   **Smallest**, **largest**, and **next** numbers control the number generation. Next is the next value to be used. Generally, the smallest is 1 and the largest is as many 9s as you have digits in the alphanumeric segment.
    -   **Continuous** does not leave gaps. Numbers assigned and then removed (journal deleted) are put into a pool or status list and get used the next time a number from this sequence is required. It’s used when continuous auditing is required; otherwise non-continuous should be used.
    -   **Manual** indicates the user will assign the number. Often companies want to assign their own customer and vendor account numbers and set those sequences to **Manual**.
9.  Next, navigate to **General ledger** \> **Journal setup** \> **Journal names**. Point out the **Voucher series** value. This is a number sequence. Select the hyperlinked value. It brings you to the **Number sequence detail** page for this number sequence. Number sequences not defined on parameter forms are often selected on other forms in the system such as this one. These are harder to find and determine where you specify them.

Summarize the session by indicating that setting up number sequences has many complexities to:

-   Avoid running out of the range of numbers allowed.
    -   Have reasonable performance. (You can set performance options.
    -   Be readable and easily identifiable in lists.

Number sequences are an integral part of finance and operations apps.
