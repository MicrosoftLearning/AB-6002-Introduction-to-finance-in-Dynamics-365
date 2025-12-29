---
lab:
    title: 'Lab 1: Personalize your workspace'
    module: 'Module 1: Describe the finance and operations apps'
---

# Module 1: Describe the Dynamics 365 finance and operations apps

## Lab 1: Personalize your workspace

## Objectives

In this lab, you will create a filtered view and add it to a workspace. Your goal is to have easy access to customers who are on hold.

## Lab Setup

- **Estimated Time**: 10 minutes

## Tasks

1.  In the **Navigation pane**, select **Modules** \> **Accounts receivable** \> **Customers** \> **All customers**.
2.  Right-click the **Account** column header.
3.  Select **Insert column**. Add the column **Invoicing and delivery on hold (Confirmation, delivery and invoicing on hold)**. You can filter the **Field** column in the list to help locate this column.
4.  Scroll the list of customers to the right to display the field you added. Hover over the leftmost edge of the I**nvoicing and delivery on hold (Confirmation, delivery and invoicing on hold)** column header until a symbol that looks like a cross with four arrow points appears. This is the Move icon. Drag the column to the right of the **Customer account** column.
5.  Hover over the **Customer group** column header until you see the downward caret, and then select the header. Set the filter to **is exactly**, then enter **10**, and select **Apply**. Now only the customers that are in **customer group 10** are displayed.
6.  Hover over the **Invoicing and delivery on hold (Confirmation, delivery and invoicing on hold)** column and add a filter for **is not All**. The customers listed have a hold of **All**.

    Note the words **Standard view\*** above the grid. The **\*** means you made changes to the form and can save them.

7.  Select the caret next to the words **Standard view** and select **Save as**.
    - In the name field, enter **Group 10 on hold**.
    - In the **Description** field, enter **Customers in group 10 on hold**.
    - Select **Save**.
8.  In the **Personalize button** group, on the **Options** menu, select **Add to workspace**.
    - Select the **Customer credit and collections** workspace.
    - Presentation should be **Tile**.
    - Select the **Configure** button.
    - Select **Yes** for **Show number count**.
    - Leave the tile size as **2x2**.
9.  In the **Personalize button** group, in the **Options** menu, select **Add to workspace**.
    - Select the **Customer credit and collections** workspace with a **List** presentation.
    - Select the **Configure** button.
    - Clear the **Currency** field selection.
    - Select the **Credit limit** field.
    - Select the **Add to workspace** button.
10. From the Navigation pane, open **Workspaces** and then select **Customer credit and collections**.
11. Expand the **Summary** FastTab if collapsed to display the tile you created. It will be the rightmost tile in this section. Select this tile. The **All customers** page is displayed with your filter.
12. Select the back arrow.
13. Review the **Collections** lists. Note that the last one is your **Group 10 on hold** list.
14. Select the **Group 10 on hold** list. The list of customers displayed are those in group 10 and have a hold.
15. Right-click the tile you created and select **Personalize**. Select **Pin to dashboard**. Select outside the **Personalize** box to close it.
16. Select **Finance and Operations** in the title bar. Scroll though the tiles until you get to **Customer credit and collections**. The **Group 10 on hold** filter name is added to the dashboard, and the count appears on the line with the filter name.




