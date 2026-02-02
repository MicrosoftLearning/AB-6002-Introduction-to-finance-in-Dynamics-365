Security

This the roles assigned to a user determine which features they can access in finance and operations apps.

**Setup**

Three user accounts are required (which is why we are doing this as a video).

-   APClerk – has roles System User and Accounts payable clerk
-   APManager – has roles System User and Accounts payable manager

Admin – this is the system administrator and already existsIn this demo, we demonstrate the security features of finance and operations apps. Each user is assigned a set of roles, and the roles have duties and privileges that determine what they can do or what is displayed in the application.

3 different users logged in:

-   The system administrator
-   An accounts payable clerk
-   An accounts payable manager

Let’s review the default dashboard and the navigation pane with the list of workspaces and modules available to each user.

Let’s start with the system administrator. This is a special account in the system with more rights than any other account. It can perform almost all functions including creating users and assigning roles. The security administrator role can also manage users and their permissions.

The default dashboard for the system administrator is full of tiles representing each of the modules available in the application. The navigation pane also has a complete list of workspaces and modules that is displayed when these lists are expanded. If we display a specific module, the menu items available show exactly what the system administrator can do. These menu items are shown or hidden based on security privileges that are defined within the security duties assigned to the role. As an example, let’s open the Dynamics 365 **Human resources** module. The system administrator has all Human resources features available.

Let’s look at the accounts payable manager next. This user works with vendors – maintaining the vendor master records, creating and reviewing journals, creating and reviewing vendor invoices. The options available on both the dashboard and the navigation pane are very limited compared to the system administrator. The accounts payable manager has several analytics tiles and menu items available such as cash overview. Still a large list of modules but certainly not as many as the system administrator. Let’s look at the vendor master. I’ll navigate to **Accounts payable \> Vendors \> All vendors**. Select the first vendor in the list to open the **Vendor details** page. Note that the **Edit** and **New** menu items are available. Now open the **Human resources** module. The accounts payable manager does not need permissions to manage Human Resources and has a limited number of features available.

Now let's look at the accounts payable clerk. This user has some of the same features available as the accounts payable manager but not all. When the user opens various pages in the system, they have more limited access – sometimes restricted to read only rather than read/write. This is the **Vendor details** page. I open it the same way as I did for the accounts payable manager by first selecting all vendors and then selecting the first vendor in the list. Note that the **Edit** and **New** menu items are **NOT** available. In this environment, the accounts payable manager can make changes to vendors whereas the accounts payable clerk can only view but not change vendor information. What about the **Human resources** module? The accounts payable clerk doesn’t even have this module in the list!

Each instance of finance and operations apps starts with a predefined set of built-in security roles, duties, and privileges. A large portion of every implementation is to use the built-in security that exists and to make changes where appropriate to match the job responsibilities of each user in the system. Every menu item can be defined as available with just Read or Read and Write privileges for each user. Finance and operations apps are extremely flexible and customizable in the security setup.
