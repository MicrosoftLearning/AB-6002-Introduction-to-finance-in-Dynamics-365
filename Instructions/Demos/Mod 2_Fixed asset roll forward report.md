# Fixed asset roll forward for Electronic reporting with export

### Prerequisite: Electronic reporting setup

The **Fixed assets roll forward** report uses the Electronic reporting (ER) framework. Before you can run the report, the **Fixed assets** model and **Fixed asset roll-forward** configurations must be imported from Microsoft Dynamics Lifecycle Services (LCS). For instructions, see Download Electronic reporting configurations from Lifecycle Services.

In this demo, we’ll explore the process of running the **Fixed asset roll forward** report and then exporting the report to Microsoft Excel from Dynamics 365 Finance.

Navigate to **Fixed assets \> Inquiries and reports \> Transaction reports \> Fixed asset roll forward**.

The **Fixed assets roll forward** report provides fixed asset data details in an easy-to-read Excel format for period closing, financial statements, and tax reporting.

In the page that appears, we’ll enter our selection for the report. In the **Parameters** section, select the **From date** and **To date** fields for the report data you want.

Next, you choose a **Currency**. We’ll select **Accounting currency**.

In the **Format mapping field,** choose the **Fixed asset roll forward configuration** that has already been configured for use. The report uses the Electronic reporting framework to generate the report. Before you can run the report, the **Fixed assets** model and **Fixed asset roll forward** configurations must be imported from the Microsoft Dataverse repository. This is generally done by an administrator and made available to end users.

You can filter the report by choosing **Records to include** in the next section of the page. You can also set the report to run in **Recurrence** by using **Batch processing**.

Select **OK**.

The report now generates and creates an Excel file based on the parameters you just set.

Open the downloaded Excel file to view the **Fixed asset roll forward** report. You can view the report and manipulate it in Excel to best meet your business requirements.

The Excel report provides beginning and ending balances for each fixed asset, along with period activity such as acquisitions, disposals, and depreciation.

Values are detailed at the asset level and summarized by fixed asset group and legal entity.

This report is a great example of the data extraction and formatting capabilities of Electronic reporting.
