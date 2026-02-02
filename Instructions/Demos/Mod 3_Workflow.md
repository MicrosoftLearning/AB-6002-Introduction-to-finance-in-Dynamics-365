# Workflow summary

**Preparation:**

1.  Add a User group in **System Administration \> Users \>User groups**. Call the group GenJrnl with description **General journal approvers**. Add users SARA,PHYLLIS, KEVIN.
2.  In the **General ledger** module, open the **General ledger workflows** page from the **Journal setup** group.
3.  Open workflow **000131** for edit. Change the assignment of the Approval step to **Participant\>User group\>GenJrnl**. **Save and close**. When prompted, indicate you want to **Activate this version**.
4.  Create a general journal using the **WFGenJrnl** journal name. **Validate\>Simulate posting**.
5.  the **General journal** menu item to go back to the list of journals. **Workflow\>Submit** to submit the journal to workflow for approval.
6.  Set up the workflow batch jobs in **System administration \> Workflow \> Workflow infrastructure configuration**. Use defaults **OK**. If you don’t do this likely the workflow will never progress.
7.  In **System administration \> Inquiries\> Batch jobs** search **Job description** field for **Contains Workflow**. If the **Workflow message processing job** has status **Withhold**, **Change status** menu item and change it to **Waiting**.
8.  **Workflow \> View history**

**Script**

In this we review the workflow history and the opilot workflow summaries. Often an administrator will be asked to explain why a workflow took so long to approve or why a workflow is failing. The workflow history with the opilot summary are key tools to determine what happened. For this example, I have a help desk ticket because a workflow failed.

Let’s open the workflow history page. It is in the **Organization administration** module here under **Workflow** and then **Workflow history**. This page is global and shows workflows from all legal entities so it doesn’t matter which legal entity we are in when we view it.

When the page opens, the default filter shows workflows that are stopped due to an error. This makes sense because that is the primary reason an administrator will view this page. The workflow we need to look at is the top onea general journal approval workflow.

When I open the page, the **Summary by Copilot** FastTab is collapsed. A summary isn’t generated until I open this FastTab. Whenever these summaries exist on a page your performance will be best if you collapse the FastTab before leaving the page and only open it when you wish to see the ummary. These Copilot summaries exist on many pages and leaving collapsed on all of them is best until you need it.

Let’s open the **Summy by Copilot** and see what it says. It shows we have a permission error for user KEVIN. This is a very common error when workflows are modified or new users are added. The users that are selected for pproval must have rights to the documents they are being asked to approve. In this example I see immediately that KEVIN is missing some privilege. The workflow can’t tell me which privilege (and hence the **Summy by Copilot** won’t tell me that either). Here I can use the system to look at KEVIN’s privileges to see if he has rights to general journals and if so, what kind of rights? He’ll need to be able to **update** journals to do the approval **Read** is not enough.

I can ask Copilot what privileges are required for the approval. Let’s use the **Copilot sidecar**. I’ll just bring it up here.

**Ask Copilot**

which privileges are required to approve a daily journal

**Copilot response**

**Privileges Required to Approve a Daily Journal Batch**

-   Approval of a general journal batch typically requires users to have specific roles or privileges, such as being an **accounting manager** or a designated approver within the system.
-   In Dynamics 365, anyone with the appropriate approval role set up in the Approval User Setup page can approve general journal batches. This setup is managed through workflows, such as the General Journal Batch Approval Workflow or the General Journal Line Approval Workflow.
-   For privileged user management, system administrators have the authority to approve or edit session requests, which may include journal batch approvals if elevated privileges are needed. Only users with the System administrator role can approve or edit privileged user session requests.
-   It is recommended that privileged accounts, which can approve sensitive transactions, are allocated only to high-privileged users and remain disabled when not in use for security and compliance purposes

**Talk to myself**

Copilot says often the approval is by an accounting manager. The approval workflow uses a user group. I know that SARA, PHYLLIS, and KEVIN are in the user group I’ve checked that before.

I can see who has the **Accounting manager** role by looking at the **Assign users to roles** page in the **Security** group of **System administration**. I’ll **Accounting manager**. OSCAR, PHYLLIS, and SARA all have this role. KEVIN does not. I can provide this list to the person that opened the help desk ticket to determine whether KEVIN should be removed from the group or provided a role similar to **Accounting Manager.**

**Summary**

This is a very simple workflow with just one stepthe approval of the general journal. Some workflows take branches, run parallel steps, stop for manual stepsthey can be very complex. When you look at the amount of information stored for this simple workflow, consider what the history would look like for a more complex workflow. **Summary by Copilot** will quickly bring you up to speed on exactly what happened with the workflownd the **Copilot Sidecar** can help you understand exactly what caused this error.

