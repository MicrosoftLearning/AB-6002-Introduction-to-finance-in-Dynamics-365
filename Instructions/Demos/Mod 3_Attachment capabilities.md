## Module 3: Describe shared features

## Demo: Attachment capabilities

In this demo, you will explore adding and viewing attachments.

**Scenario:**

You are an accounts payable manager. You just received a W-9 form from Acme Office Suppliers, vendor 1001. You want to determine if a W-9 is already on file and upload this latest one, removing the older version if one exists.

**Preparation:**

1.  Create a file named **W9**. Download a copy of the blank form from the government by going to Form W-9 (Rev. March 2024).
2.  Put the file in a place on the virtual machine where you can find it easily.

**Demo:**

1.  Open Dynamics 365 Finance. Change the company to **USMF** if you’re not already in this legal entity.
2.  Navigate to **Accounts payable \> Vendors \> All vendors**.
3.  Select vendor number **1001** to open the **Vendor detail** page.
4.  Expand the **Tax 1099 FastTab** if collapsed. Your company has a policy to set the **W-9 received** flag when you attach a W-9. The flag is set to **No**, so it appears none is on file.
5.  Review the **Attachment** icon (paper clip). It has a “0” on it. Explain that this means there are no attachments for this vendor.
6.  Select the paper clip to open the attachment page.
7.  Select **New \> File**. Explain that often companies will create a document type for W-9s. Since this company doesn’t have one, you’ll use **File**.
8.  Select the **Browse** button and select the W-9 file you stored on the image.
9.  Expand the **Preview** FastTab if collapsed. Show the preview of the document. Describe how being able to preview documents can save a lot of time when validating a document or when searching through all attachments for a specific one you want to open.
10. Select the **Open** menu item. This downloads the document so you can view it in the PDF viewer.
11. Close the attachment page by selecting the **Back** arrow.
12. Focus on the paper clip again and show that there is a 1 on it now to indicate the vendor has one attachment.
13. Change the **W-9 received** flag to **Yes** in the vendor’s **Tax 1099 FastTab**.

**Post demo discussion:**

Which documents in finance and operations apps would you expect to attach files to? Which types of files would you attach?

-   Vendor invoice PDFs can be attached to the vendor invoices in finance and operations apps.
-   Email notifications of payments can be attached to the payment record.

Some attachments that are created by finance and operations apps can be automatically placed on documents with customizations to remove the manual attachment.

