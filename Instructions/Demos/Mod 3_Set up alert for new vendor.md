Module 3: Describe shared features

Demo: Set up an alert when a new vendor is created

In this demo, you will add an alert when a new vendor is created and show how the alert is triggered and then notifies you.

**Scenario:**

You are an accounts payable manager. You are responsible for collecting W-9 forms from each vendor. You decide to create an alert that notifies you when each new vendor record is created. You can then contact the vendor and request the W-9 form.

**Preparation:**

1.  Go to **System administration** \> **Inquiries** \> **Batch jobs.**
2.  Filter the **Job description** column for **contains Alert**. Find the job **Change based alerts**.
3.  If the job is in status **Withold**, select the **Change status** menu item and change the status to **Waiting**. If the job is NOT run by using an **Admin account**, it likely won’t work.
4.  If the alerts don’t trigger, create a new job by going to **System administration** \> **Alerts** \> **Change based alerts**. Set it up with **NO END DATE** and to run every **1 minute**.

**Demo:**

1.  Open Dynamics 365 Finance. Change the company to USMF if you’re not already in this legal entity.
2.  Navigate to **Accounts payable** \> **Vendors** \> **All vendors**.
3.  Select **Options** \> **Share** \> **Create a custom alert.**
4.  In the **Create alert rule** dialog, show that the table name is **Vendors** and the default **Event** is **Record has been created**. This is exactly what you need so you can leave this as defaulted.
5.  Expand the **Alert me for** FastTab if collapsed. It should read **All records in Vendors**. Since you are responsible for just this one legal entity, leave the **Organization wide** option set to **No**. Explain that if you were in a Central AP group handling all the legal entities, you would set this option to Yes.
6.  Expand the **Alert me until** FastTab if collapsed. Select **No end date** (this is the default).
7.  Expand the **Alert me with** FastTab if collapsed. The default subject is fine. You will use just the **Action center** to notify you, but explain that you can email as well. If you want the email, you need to change the **Send email** option to **Yes** and add an **Email recipients** list**.**
8.  If asked, explain that **Send externally** is used to notify other systems. This type of notification is discussed in another module.
9.  Select **OK** to close the dialog and save the alert.
10. Now it is time to trigger the alert. Select the **New** menu item on the **All vendors** page.
11. Enter vendor account **ALRT0001**, vendor name Liberty's Delightful Sinful Bakery & Cafe, and select Group **20**. Select **Save** or close the vendor page. Wait a few minutes. The Alert process is a scheduled batch job and needs to run before you get a notification. You can select **Refresh** in the upper right of the page to refresh the Action center notifications.
12. Review your existing alerts by selecting **Options** \> **Share** \> **Manage my alerts**. The new vendor alert you just created will appear.
13. System administrators can review all alerts by navigating to **System administration** \> **Setup** \> **Alert** rules. Show this form. Indicate that the administrator can combine the email user list from multiple alerts into one to improve performance. The administrator can also create alert rules for others. Only one person receives a notification in the Action center.

**Post demo discussion:**

Are there other alerts that might make sense for an Accounts payable manager to create?

-   Invoice postings (if not the one to approve)
-   Payments (if not the one to approve)

Inquiries and reports can provide historical information. Alerts are for when you want **immediate** notification, so do not overuse!
