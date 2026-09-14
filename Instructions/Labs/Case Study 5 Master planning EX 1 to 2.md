---
lab:
  title: Case study 5 Master planning
  module: 'Module 5: Implement master planning '
  description: Case study 5 Master planning ============================
  duration: 20 minutes
  level: 200
  islab: true
---

Case study 5 Master planning
============================

Objectives
----------

- *Firm and review a planned purchase order, change it to production, and verify the change.*

- *Create a planning group, assign an item allocation key, and run the intercompany master plan.*

Exercise \#1 Process and view planned orders
--------------------------------------------

*Objective: Firm and review a planned purchase order, change it to production, and verify the change.*

The planning manager in USMF wants to know how to setup, manage, and use the master planning module, as well as how to process planned orders.

To firm planned orders, He will need to be sure that the master planning is running correctly, or there are some planned orders in the form that you can use.

You were called to help the planning manager to perform the above tasks

You will need to use the following:

- Firm a planned purchase order.

- Review the purchase order.

- Change the planned purchase order type.

- Review the planned order and verify the change

### Firm a planned order

1. Open **Master planning \> Master planning \> Planned orders**.

2. On the **Planned orders** page, select the line for order number **004126**. (or an available Planned purchase order with a small requirement quantity and a selected vendor.)

3. Select the **Firm** button in the action pane.

4. On the **Firming** page, in the **Update marking** field, select **Standard**.

5. Select **OK**.

### Review the purchase order

1. Open **Procurement and sourcing \> Purchase orders \> All purchase orders**.

2. On the **All purchase orders** page,  filter the list and find the firmed order.

3. Verify the firmed order is now listed with a status of **Open order**.

4. Close the pages.

### Change a planned order type

You need to change the planned order type for an order.

1. Open **Master planning \> Master planning \> Planned orders**.

2. On the **Planned orders** page, select the line for order number **004137**. (or an available Planned purchase order with a small requirement quantity and a selected vendor.)

3. Select the **Planned order** tab in the action pane.

4. Select the **Change to …** drop-down arrow in the **Maintain** area.

5. Select **Planned production order**.

6. On the **Change to planned production order** pane, select **OK**.

### Review the planned order and verify the change

1. On the **Planned orders** list page, verify that the **Reference** field has been updated to **Planned production orders** for order number **004137**.

2. Close the pages.

Exercise \#2 Create and run intercompany master plans
-----------------------------------------------------

*Objective: Create a planning group, assign an item allocation key, and run the
intercompany master plan.*

You were called to help the materials and production scheduling manager, to
develop a new intercompany planning group.

Assemblies are shipped from DEMF to USMF.

While at USMF they are painted and finished with the North American logo.

Then they are transferred to the USRT operation for sale.

He wants to use the Plans 20, DynPlan, and MasterPlan respectively to accomplish
this goal.

He would like to validate the Intercompany master planning parameters and
perform some setups before running the intercompany master plan.

Then he would need to run the intercompany plan using the planning group that he
will create. Finally he would want to view the results in the intercompany
supply and demand form.

Would you assist the planning manager in doing the following?

- Create an intercompany planning group.

- Assign an item allocation key.

- Run an intercompany master plan.

### Create an intercompany planning group

1. In the **USMF**, open **Master planning \> Setup \> Intercompany planning groups.**

2. Select **+ New** on the Action pane.

3. Enter **Intercompa** in the **Name** field and **Intercompany Extended Group** in the description.

4. Select **Save**.

5. Select **+ New** on the tool bar for **Intercompany planning group members** section.

6. Select **DEMF** in the **Legal entity** field.

7. Enter **0** in the **Scheduling sequence** field.

8. Select **20** for the **Master plan** field.

9. Leave **Automatic Copy to Static Plan** and **Automatic Copy to Dynamic Plan** checkboxes blank.

10. Select **Save**.

### Assign item allocation key

1. Select **Master Planning \> Setup \> Demand Forecasting \> Item allocation keys**.

2. Select **Wizard** and select **Next**.

3. Select **Audio** from **Item Group** drop-down menu and select **Next**.

4. Type **Audio Group** in **Name** box.

5. Select **Next**.

6. Select **Next** on the **Overview** page after verifying information is correct.

7. Select **Finish** on the **Completed** page after verifying information is correct.

8. Switch to the **DEMF** company. Repeat steps 1 - 7.

9. Switch to the **USMF** company.

10. Select **Master Planning \> Setup \> Intercompany planning groups.**

11. Select **Intercompa** from the Intercompany planning Groups list (record created from the previous task) and select the **Item Allocation Keys.** related to the **DEMF** from the Intercompany planning group members area.

12. Select **Audio** under the **UNASSIGNED ITEM ALLOCATION KEYS** box.

13. Select **\>** to move it to the **ASSIGNED ITEM ALLOCATION KEYS** box.

### Run an intercompany master plan

1. As the materials and production manager, you will need run the intercompany plan utilizing the intercompany planning group that you created earlier. View the results in the intercompany supply and demand form.

2. In the USMF, go to **Master Planning** \> **Master planning** \> **Run** \> **Intercompany master planning**.

   > [!NOTE]
   > If you cannot run the intercompany master plan because Planning Optimization is enabled, review the remaining steps to understand the process without completing the actions.

3. Select **Intercompa** for **Intercompany planning group**.

4. Select **2** for **Number of intercompany planning iterations**.

5. Select **Regeneration** for **First iteration**.

6. Select **Net change** for **Subsequent iteration**.

7. Select **Track processing time** setting slider to **No**.

8. Set **Number of threads** to **0**.

9. Select **Run in the background.**

10. Select **OK**.

11. Open **Master planning \> Inquiries and reports \> Intercompany master planning \> Intercompany supply and demand.**
