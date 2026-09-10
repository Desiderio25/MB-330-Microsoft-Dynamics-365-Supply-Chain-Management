---
lab:
  title: Case study 3A Procurement and sourcing
  module: 'Module 3: Implement and manage supply chain processes '
  description: The employee must identify a vendor for the request and the quantity required. The employee do not know the actual part number, so you will use a procurement category instead.
  duration: 30 minutes
  level: 200
  islab: true
---

Case study 3A Procurement and sourcing
======================================

Objectives
----------

- *Create a purchase requisition using a procurement category and then submit
    and approve the purchase requisition*

- *Create a request for quotation, reply and accept a vendor’s reply.*

- *Create a purchase requisition permission policy with a new requester name
    and create an office supplies purchasing policy.*

- *Create a purchase order for two different items, each to be delivered to a
    different site.*

- *Create a charge code for vendor transport charges on various items.*

- *Create a vendor charge group and assign it to two vendors.*

- *Create an item charges group and use it to create an automatic charge.*

- *Set up change management so purchase orders are approved prior to
    confirmation.*

- *Create a purchase order from on a trade agreement based on value or
    quantity.*

- *Create a trade agreement for domestic vendors that specifies a fixed price
    for a certain item.*

- *Create a guest user for a supplier so they can access the system.*

Exercise \#1 Create, submit, and approve a purchase requisition
---------------------------------------------------------------

*Objective: Create a purchase requisition using a procurement category and then
submit and approve the purchase requisition.*

An employee of the IT department of USMF wants a longer HDMI cables for the new
office and meeting rooms. a purchase requisition will have to go through the
internal approval process before the items are purchased.

The employee must identify a vendor for the request and the quantity required.
The employee do not know the actual part number, so you will use a procurement
category instead.

**The IT employee asked you to help. What system features you would show and
help her to use?**

### Create and process a purchase requisition

1. In Microsoft Dynamics 365 Supply Chain Management, go to **Procurement and sourcing \> Purchase requisitions \> All purchase requisitions**.

2. Select **+ New**.

3. For **Name** enter **New HDMI Cables**.

4. Select **OK**.

5. For **Reason** select **General supplies**.

6. For **Details** enter **New, longer HDMI cables**.

### Add an item to the purchase requisition

1. Select **Add products** in the **Purchase requisition lines** FastTab.

2. Expand the **Office Machines** procurement category, and then select **Computers**.

3. Under **Select From Filtered List**, expand **Add unlisted product to lines**.

4. For **Product name** enter **24in HDMI Cable**.

5. For **Unit** enter **ea**.

6. Select **OK**.

7. Verify the **Lines to add to purchase requisition** section.

8. For **Product name** enter **24-inch HDMI cable**.

9. For **Quantity** enter **5**.

10. Unit price: Enter **41.49**.

11. For **Vendor Account** select **100001** (Syrup Supplies Co.).

12. Select **OK**.

### Submit the purchase requisition created in the previous practice for approval, and perform the approval process

1. Go to **Procurement and sourcing** \> **Purchase requisitions** \> **All purchase requisitions**.

2. Open the draft purchase requisition created in the previous practice.

3. Select **Workflow** at the top, and then select **Submit**.

4. For **Comment** enter **Request for longer HDMI cables.**

5. Select **Submit**.

6. Select **Workflow \> Workflow history**

7. Select **Refresh** a few times and wait until the **Work items** section shows records.

8. Select **Reassign** button.

9. Select **Admin** in the **User field.**

10. Select **Reassign**. Notice the work item has been reassigned to a new worker.

11. Select **Refresh**.

12. Close the **Workflow history** page.

    > [!NOTE] 
    > After you submit the purchase requisition, its status might change to **In review** without a workflow work item being generated. If the **Work items** section on the **Workflow history** page is empty, the **Reassign** and **Approve** actions aren't available. In this case, continue to the next exercise.

### Approve the purchase requisition

1. Select **Workflow** at the top, and then select **Approve**.

2. Comment: Enter **Approved.**

3. Select **Approve**

Exercise \#2 Create, reply and accept a request for quotation (Bonus)
---------------------------------------------------------------------

*Objective: Create a request for quotation, reply and accept a vendor’s reply.*

After the Purchase requestion was approved, the Procurement department found
that there were a lot of other requests for the same type of cables, so they
have decided to buy a larger quantity to benefit from bulk pricing.

The purchase clerk must create and process a request for quotation for a
quantity of 500 of A0001 HDMI 6 foot cables that will be sent to two different
vendors, US-111 (Contoso Office Supply) and US-103 (Rain Projectors), and it
should be set to update vendor replays in order to choose the best offer.

You will have to do the following:

- Create the request for quotation and send to the appropriate suppliers

- Add a line to the request for quotation.

- Reply to a request for quotation.

- Accept a vendor’s reply.

### Create the request for quotation and send to the appropriate suppliers

1. Go to **Procurement and sourcing** \> **Requests for quotations** \>
    **All requests for quotations**.

2. Select **+ New**.

3. For **Purchase type** select **Purchase order**.

4. For **Document title**, enter **HDMI Cables**.

5. For **Site**, select **1** (Home speakers production).

6. For **Warehouse**, select **13** (Site 1 – Finished Goods).

7. Select **OK**.

### Add a line to the request for quotation

1. If necessary, select **Add line** to add a line to the list.

2. For **Line type**, select **Item**.

3. For **Item number**, select **A0001** (HDMI 6’ Cables).

4. For **Quantity**, enter **500**.

5. Select **Save**.

6. Select **Header**.

7. Verify the **Vendor** FastTab.

8. If necessary, select **Add** to add a line to the list.

9. For **Vendor account**, select **US-111** (Contoso office supply).

10. Select **+ Add**.

11. For **Vendor account**, select **US-103** (Rain Projectors).

12. Select **Save**.

13. Select **Quotation** at the top, and then select **Send** under the
    **Process** section.

14. Review both of the previously selected vendors.

15. Select **OK**.

### Reply to a Request for Quotation

Update the request for the quotation created in the previous practice with the
vendor responses.

1. Make sure that the permission to edit vendor bids is setup. Go to the **Procurement and sourcing** \> **Setup** \> **Procurement and sourcing parameters**.

2. On the **Request for quotations** tab, toggle on the **Purchaser can edit vendors bid** option to **Yes**.

3. Select **Save**.

### Process the quotation for US-103. Enter the vendors’ replies to the request for quotation

1. Go to the **Procurement and sourcing \> Requests for quotations \> All requests for quotations**.

2. Open the request for quotation previously created.

3. Select **Header**.

4. Go to the **Vendor** FastTab.

5. Select the **Request for quotation** number for **US-111** (Contoso office supply).

6. Select **Manage reply**. Select the **Edit** at the top, from the drop-down menu select **Edit RFQ reply**  

7. For **Quantity**, enter **500**.

8. For **Unit**, enter **ea**.

9. For **Unit price**, enter **10.00**.

10. Select **Save**.

11. Close the **Request for Quotation bid** page.

12. Close the **Request for Quotation** page.

13. Select the **Request for quotation** number for **US-103** (Rain Projectors), on the **Vendor** FastTab

14. Select **Manage reply**. Select the **Edit** at the top, from the drop-down menu select **Edit RFQ reply**

15. For **Quantity**, enter **500**.

16. For **Unit**, enter **ea**.

17. For **Unit price**, enter **8.00**.

18. Select **Save**.

19. Close all the pages.

### Accept a vendor’s reply

1. Go to the **Procurement and sourcing \> Requests for quotations \> All requests for quotations**.

2. Open the request for quotations created in the previous practice.

3. Select **Header**.

4. Locate the **Vendor** FastTab.

5. Select the **Request for quotation** number for **US-103** (Rain Projectors).

6. Select **Manage reply**. Select **Edit** at the top, from the drop-down menu select **Edit RFQ reply**

7. Select **Submit** from the top menu.

8. In the confirmation dialog, select **Close**.

Exercise \#3 Create purchase requisition and purchasing policies (Bonus)
------------------------------------------------------------------------

*Objective:  Create a purchase requisition permission policy with a new
requester name and create an office supplies purchasing policy.*

The purchasing manager decided to make some updates.

He wants to update the requisitions permission policy with a new requester name
and create a new purchasing policy for office supplies with an additional
category.

He reached out for help and you will have to do the following:

- Create a purchase requisition permission policy.

- Create a purchasing policy.

### Create a purchase requisition permission policy

1. Go to **Procurement and sourcing \> Setup \> Policies \> Purchase requisition permissions**

2. Select **Mike Danseglio** in the list of workers.

3. Change to the **Requester** FastTab.

4. Select **+ Add**.

5. For **Name**, search for **Susan Burk** and then **Select**.

6. Select **Save**.

### Create a purchasing policy

1. Go to the **Procurement and sourcing \> Setup \> Policies \> Purchasing policies**.

2. Select **Procurement Policy USMF**.

3. Expand the **Policy rules** FastTab.

4. In the **New** tab on the Action Pane, select **Policy**.

5. For **Name**, enter **Office Supplies**.

6. For **Description**, enter **Office supplies policies**.

7. For **Policy rule type**, select **Category access policy rule(x)**.

8. Select **Create policy rule** in the **Policy rules** section on the right.

9. Select **Office and Desk Accessories** in the **Available Categories** list.

10. Select the right arrow button.

11. Select **OK**.

12. For **Effective date**, select a future hour.

13. Select **Save**.

Exercise \#4 Create a purchase order for delivery to multiple sites
-------------------------------------------------------------------

*Objective: Create a purchase order for two different items, each to be
delivered to a different site.*

The purchasing clerk at USMF wants to create one purchase order for a quantity
of 5 of item T0003 (surround sound receiver) from Acme Office Supplies, to be
delivered today to Site 1, and a quantity of 5 of item M1101 (foam reacting
agent) to be delivered to the Quality Testing Center, 123 W. Cherry Street, zip code 83642.

He is not clear how to perform this using the system and asking your help

**What would you do?**

### Create a purchase order

1. Go to the **Procurement and sourcing** \> **Purchase orders** \> **All purchase orders**.

2. Select **+ New**.

3. For **Vendor account** select **1001** (Acme Office Supplies).

4. For Delivery date, expand the **General** tab, verify the current date in the **Requested receipt date** field (this should be the default value).

5. Select **OK**.

6. Add items to the purchase order:

    1. For **Item number** select **T0003** (Café A -200 Automatic).

    2. For **Quantity** enter **5**.

    3. For **Unit** enter **ea**.

    4. Select **+ Add line**.

    5. For **Item number** select **M1101** (Foam reacting agent).

    6. For **Quantity** enter **5**.

    7. For **Unit** enter **PL**.

7. Select delivery addresses for the items:

    1. Select the line for item **T0003** (Café A -200 Automatic) in the
        **Purchase order lines** FastTab.

    2. Expand the **Line details** FastTab.

    3. Select the **Address** tab.

    4. Select **Contoso USMF HQ** in the **Delivery address** field.

    5. Select the line for item **M1101** (Foam reacting agent) in the
        **Purchase order lines** FastTab.

    6. Select the **Line details** FastTab.

    7. Select the **Add address** button (**+**) to the right of the **Delivery address** field.

    8. Enter **Quality Testing Center** in the **Name or description** field.

    9. Enter **83642** in the **Zip/postal code** field.

    10. Enter **123 W. Cherry Street** in the **Street** field.

    11. Select **OK**.

8. Select **Save**.

9. On the Action pane, select **Purchase**

10. Select **Actions** > **Confirm**.

11. Select **OK**.

12. On the Action Pane, select **Receive**.

13. Select **Generate** \> **Product receipt**.

14. Select **Registered quantity** in the **Quantity** field.

15. In the **Product receipt** field, enter the product receipt number. For
    example, enter **PR123**.

16. Select **OK** to post the product receipt.

17. Close all pages.

Exercise \#5 Create a charges code
----------------------------------

*Objective:  Create a charge code for vendor transport charges on various
items.*

The accounts payable coordinator at Contoso Entertainment Systems USA must
complete some setups for transport charges added to various items by the vendor.

She can do this in the system by creating a charges code with the following
specifications:

- Name of the charges code: TRANSTO

- Description: Transportation Fee to our sites

- Account: 411400

- This fee does not require an item sales tax group.

> **She asked for your help to show her how this charges can be configured.
> What would you do?**

### Create a charges code

1. Go to the **Accounts payable** \> **Charges setup** \> **Charges code**.

2. Select **+ New**.

3. For **Charges code**, enter **TRANSTO**.

4. For **Description**, enter **Transportation Fee to our sites**.

5. Go to the **Debit** section.

6. For **Type**, select **Ledger account**.

7. For **Posting**, select **Payment fee**.

8. For **Account**, select **411400**.

9. Go to the **Credit** section.

10. For **Type**, select **Customer/Vendor**.

11. Select **Save**.

Exercise \#6 Create a vendor charges group and assign to vendors (Bouns)
------------------------------------------------------------------------

*Objective:  Create a vendor charge group and assign it to two vendors.*

The accounts payable administrator at Contoso Entertainment Systems USA, wants
to make updates for Fabrikam supplier, that has two vendor accounts from which
Contoso purchases items.

Fabrikam recently imposed an additional 15 percent freight charges for all
purchase orders.

He is not sure how to set up a new charges and not quite sure how to assign to
the supplier accounts.

You will have to do the following:

- Create a vendor charges group.

- Update vendors to use the new vendor charges group

### Create a Vendor Charges Group

1. Go to the **Accounts payable** \> **Charges setup** \> **Vendor charges group**.

2. Select **+ New**.

3. For **Charges group**, enter **06**.

4. For **Description**, enter **Freight 15%**.

5. Select **Save**.

### Update vendors to use the new vendor charges group

1. Go to the **Accounts payable \> Vendors \> All vendors**

2. Open the vendor record for vendor **US-101** (Fabrikam Electronics).

3. Select **Edit**.

4. Expand the **Purchase order defaults** FastTab.

5. For **Charges group**, select **06** (Freight 15%).

6. Select **Save**.

7. Close the vendor record.

8. Open the vendor record for vendor **US-104** (Fabrikam Supplier).

9. Select **Edit**.

10. Open the **Purchase order defaults** FastTab.

11. For **Charges group**, select **06** (Freight 15%).

12. Select **Save**.

13. Close the vendor record

Exercise \#7 Create an automatic charge (Bonus)
-----------------------------------------------

*Objective:  Create an item charges group and use it to create an automatic
charge.*

The accounts payable coordinator at Contoso Entertainment Systems USA, wants to
make updates to vendor charges.

Datum Receivers (US-105) applies a 15 percent freight charge for all orders due
to the large quantity and weight of items we buy.

Since this charge only applies to US-105 and it will apply to every order, you
need to help the coordinator to set up an automatic charge for vendor group (06)
and the item charges group (123).

You will have to do the following:

- Create an item charges group.

- Create an automatic charge.

### Create an item charges group

1. Go to the **Accounts payable** \> **Charges setup** \> **Item charge groups**.

2. Select **+ New**.

3. For **Charges group**, enter **123**.

4. For **Description**, enter **15% Freight Charge**.

5. Select **Save**.

### Create an automatic charge

1. Go to the **Accounts payable** \> **Charges setup** \> **Automatic charges**.

2. For **Level**, select **Line**.

3. Select **+ New**.

4. For **Account code**, select **Group**.

5. For **Vendor relation**, select **06** (Freight 15%).

6. For **Item code**, select **Group**.

7. For **Item relation**, select **123** (15% Freight Charge).

8. Select **Save**.

9. Select **Add** in the **Lines** FastTab.

10. For **Charges code**, select **TRANSTO** (Transportation Fee).

11. For **Category**, select **Percent**.

12. For **Charges value**, enter **15.00**.

13. Select **Save**.

Exercise \#8 Approve purchase orders prior to confirmation (Bonus)
------------------------------------------------------------------

*Objective:  Set up change management so purchase orders are approved prior to
confirmation.*

Contoso has decided that all office supply purchase orders from supplier 1001
should be approved prior to confirmation. They asked you to activate the change
management feature for Supplier 1001.

You will have to do the following:

- Set up change management against Supplier 1001 only.

- Configure change management for a vendor.

### Set up change management against Supplier 1001 only

1. Go to **Procurement and sourcing \> Setup \> Procurement and sourcing parameters**.

2. Select the **General** tab on the left.

3. On the **Change Management for Purchase Orders** section,  select **Yes** for **Allow override of settings per vendor**.

4. Select **Save**.

### Configure change management for a vendor

1. Go to **Procurement and sourcing \> Vendors \> All vendors**.

2. Open the vendor record for vendor **1001** (Acme Office Supplies).

3. Open the **Purchase order defaults** FastTab.

4. Select **Edit**.

5. Go to the **Change Management for Purchase Orders** section in the **Purchase order defaults** FastTab.

6. For **Override settings**, select **Yes**.

7. For **Activate change management**, select **Yes**.

8. Select **Save**.

Exercise \#9 Create trade agreements for vendors
------------------------------------------------

*Objective: Create a trade agreement for domestic vendors that specifies a fixed
price for a certain item.*

The company managed to standardize the purchase price for item A0001 with all
domestic vendors to be \$8.26. You needto help the purchase manager to record
this purchase price using a trade agreement journal, so that whenever a purchase
order is created for item A0001 and the vendor is from the domestic vendors, the price will default to \$8.26.

### Create a Trade agreement for a vendor

1. Go to **Procurement and sourcing** \> **Prices and discounts** \> **Trade agreement journals**.

2. Select **+ New**.

3. For **Name**, select **S_Price** for Sales price adjustment

4. Select the **Lines** button to open the journal.

5. For **Relation**, select **Price (purch.)**.

6. For **Account code** or **Party code type**, select **Group**.

7. For **Account selection**, select **Domestic** vendors.

8. For **Item code/Product code type**, select **Table**.

9. For **Item Relation**, select **A0001, HDMI 6' Cables**.

10. For **Site**, enter or select **1**.

11. For **Warehouse**, enter **13**.

12. For **From**, enter **1**.

13. For **Amount in currency**, enter **8.26**.

14. Expand the **Details** tab.

15. For **From date**, select **February 15, 2017**.  

16. Select **Validate \> Validate all lines**.

17. Select **OK**.

18. After successful validation, select **Post**.

19. Select **OK**.

19. Close all pages.

Exercise \#10 Create a purchase order based on a trade agreement
----------------------------------------------------------------

*Objective: Create a purchase order from on a trade agreement based on value or
quantity.*

The purchasing manager always try to negotiate with vendors and create an
agreed-upon purchasing price list, discounts, and agreements for products that
are frequently purchased from a specific vendor.

Often contracts with vendors can be created to get the best prices for a
specific commitment either based on value or quantity.

In this case the purchase manager made an agreement on a price for 100 of item
number D0002 and would like to use the system to record this agreement.

**You were asked to help the purchase manager and show how this can be recorded.
What would you do?**

### Create a purchase agreement

1. Go to the **Procurement and sourcing \> Purchase agreements \> Purchase agreements**.

2. Select **+ New**.

3. For **Vendor account** select **US-104** (Fabrikam Supplier).

4. For **Purchase agreement classification**, select **General purchases**.

5. Expand the **General** FastTab.

6. For **Document title**, enter **General Purchase**.

7. For **Default commitment**, select **Product quantity commitment**.

8. Select **OK**.

### Add an item to the purchase agreement

1. Select **Add line** in the **Purchase agreement lines** FastTab to create a line.

2. For **Item number**, select **D0002** (Cabinet).

3. For **Site**, select **1** (Home speakers production).

4. For **Warehouse**, select **13** (Finished Goods).

5. For **Quantity**, enter **100**.

6. For **Unit price**, enter **145.50**.

7. For **Expiration date**, select the end of the next month.

8. Select **Save**.

   > [!NOTE] 
   > If any required columns are not displayed, select the **Grid options (...)** button on the right side of the grid, select **Insert columns...**, and then add the missing columns.

### Confirm the purchase agreement

1. Select **Purchase Agreement** at the top, and then select **Confirmation**
    under the **Generate** section.

2. For **Print report**, select **Yes**.

3. Select **OK**.

4. Close all pages
