Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.5.1Beta
May 14, 2010
----------------------------------

This is the beta release in the 3.5.1 release cycle. While this
is primarily a bug fix release, the beta includes a handful 
of new features--as well as the ability to add the following new 
packages available for download from the PostBooks project site
on SourceForge:

xTuple Desktop
  * Spec: http://www.xtuple.org/issuetracker/view.php?id=10974

Time and Expense (Lite version
  * Full spec: http://www.xtuple.org/ProjectTimeExpense

----------------------------------

The following features and bug fixes have been added to the
applications since the release of 3.5.0. Additional detail
for each item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
"Changelog" option.


New Features:

* [Accounting] Add ability to view all open payables on AP Open
Items by Vendor Report
* [Accounting] New API view for apmemo based on armemo
* [Accounting] Port #10751 to core: print customer statements
using point in time "As of" date for xTuple 3.5
* [Accounting] User Costing Elements And Accounts Change
* [CRM] Add documents tab to contact
* [CRM] Add documents tab to opportunity
* [CRM] Add documents tab to To-Do Item
* [CRM] Add documents tab to project
* [Inventory] Add an inventory trans value and ability to filter
inventory history by order type
* [Manufacture] Add documents tab to work order
* [Manufacture] Add the ability to filter work orders by status
on work order schedule by parameter list
* [Purchase] Add documents tab to purchase order
* [Purchase] Make Purchase Variance Reports show Variances
* [Purchase] Allow Part Vouchered PO's to be edited
* [Schedule] Allow planned order by planner code to be filtered
by order type
* [System] Allow XML Import of files with embedded DTD

Bug Fixes:

* [Accounting] Error messages lead to crash when creating tooling
ite
* [Accounting] Cannot Drill back to Original PO from General
Ledger Transaction Report
* [Accounting] Tax Breakdown does not match invoice tax
* [Accounting] Revision - relation error
* [Accounting] Can't select CC as bank account type, creates
confusion when setting up credit card configuration
* [Accounting] Sales credit memo total initially does not include
freight
* [Accounting] Vendor Workbench Open Balance field doesn't refresh
* [Accounting] Apply to balance on AP credit memo: wrong
calculation
* [Accounting] Open Vouchers tab on AP WB - New should carry
through Vendor selection
* [Accounting] Status on misc. A/P credit memo should be disabled
* [Accounting] Print report of Invoice Information doesn't display
Invoice amount
* [Accounting] Print Check Run doesn't print the checks
* [Accounting] OrderCluster ignores default order type when setId
is called without extra option
* [Accounting] CSVImport - GL account type is not populated upon
import
* [Accounting] Select order for billing - select balance does not
select fully shipped kit
* [Accounting] Cannot use Edit and Delete buttons on cash receipt
Misc. Distribution tab
* [Accounting] A/R workbench radio buttons allow multiple
selections
* [Accounting] invoice item window and api.invoiceline view do not
enforce item_fractional
* [Architectural] Main window launches at top of screen so the
window handle is out of reach (Mac only)
* [CRM] Unable to Edit/View the file attached to an Incident
* [CRM] Attempting to View Contact, attached on Documents Tab,
causes application crash
* [CRM] To-dos windows opening extremely large
* [CRM] Irrelevant label name is displayed on contact screen when
selecting the name from contact screen
* [CRM] Blank contact fields are being displayed upon canceling
the "Contact" dialog
* [CRM] Field missing on recurring widget in incident and invoice
* [CRM] Start and End dates are not displayed in print report of
To-Do list items by user and incident
* [CRM] Opportunity list report not printing all data
* [CRM] It's possible to edit and save, the recurrence of Project,
in "view" mode
* [CRM] To-Do list Items not immediately displayed while creating
a new Incident
* [CRM] Can't un-share a shared filter when managing
* [Inventory] Packing List Batch Screen Does not allow Single
Packing List Print (only Batch)
* [Inventory] Using standard cost on counts for avg. cost items can
lead to lock ups
* [Inventory] No privilege check for altering date in issue
material to work order
* [Inventory] Printed Inventory Availability Report doesn't display
the filter headers in consistent with the selected filters
* [Inventory] Printed Expired Inventory report doesn't display the
filter headers in consistent with the selected filters
* [Inventory] Sales Reservations are not reverted back if an item
issued to shipping is returned
* [Inventory] Can't save Cost Category on mfg if transfer in not
enabled
* [Inventory] It is not possible to edit Transfer Order
* [Inventory] Shipping Information window does not support Transfer
Orders
* [Inventory] KIT Item Type Not Supported in API
* [Inventory] Focus changes to Inventory UOM when Class Code
changed on Item screen
* [Inventory] Update Item Control by reorder level displays error
message
* [Inventory] Count tag edit list % variance has incorrect
formatting
* [Inventory] Scrap qty. field misaligned and too big
* [Inventory] Item site Standard Job radio button enabled in view
mode
* [Manufacture] Adjust Work Order Time Clock Entry still does not
work
* [Manufacture] SQL error in PostBooks on screen work order
material requirements but work order
* [Products] Print report of kit type item master doesn't
completely display item type
* [Products] Get warning message that Tooling cannot have BOM
* [Products] Cannot add tooling item to pick list
* [Products] Inconsistency around selling of tooling items
* [Products] Barcode Editable in View Mode
* [Purchase] Drop Ship Line Item Characteristics Don't follow to
Purchase Order
* [Purchase] New vendor number field does not allow for spaces
* [Purchase] Quote does not support drop shi
* [Purchase] Receipts and returns by vendor doesn't work
* [Purchase] Cannot post voucher with po line freight
* [Purchase] Purchase order line changelog incomplete
* [Purchase] Saving Purchase order line Item for �Tooling� item
generates DB log error
* [Purchase] Currency column blank on Purchase Price Variance by
Item display
* [Purchase] Qty Box Height Inconsistent on Purchase Request
Screen
* [Purchase] Purchase order open item is not functional
* [Purchase] Vendor notes Editable in view mode
* [Purchase] Item source Barcode can be edited in view mode
* [Purchase] Copying a purchase order doesn't copy vendor
information
* [Purchase] Drop Ship does not reverse shipment when correcting
receipts
* [Purchase] Vendor Information Workbench does not check for
privileges
* [Sales] Alternate Grace days does not refresh when toggling
between customers in WB
* [Sales] Item list not correct in S/O when item is exclusive and
Price Schedule assigned to Ship To
* [Sales] calcrataxamt() does not caclulate properly
* [Sales] Drop shipping does not work for kit components
* [Sales] �Quote Lookup By Item� screen doesn't display quotes
for prospects
* [Sales] Total amount of unposted CM not same as detail
* [Sales] Order Entry starting point inconsistent
* [Sales] It is possible to create blank Ship-To address
* [Sales] Quote header not getting populated with billing contact
email
* [Sales] Converting Sales Order from Quote does not check unique
cust/po combination
* [Sales] Canceling a sales order line item doesn't recalculate
freight amount
* [Sales] Remove Percent literal from Update List Price
* [Sales] Customers and Ship to Addresses are deleted without
confirmation
* [Schedule] Sales order edit allowed without that privilege
being grante
* [Schedule] Running Availability screen doesn't display the
details of item
* [System] Enable BBOM does not stay checked, marked as true in
metric table
* [System] Contact lookup missing on employee
* [System] ViewPackages priv overruled by admin role?
* [System] Enable Shipping by Customer options shown but not
functional
* [System] Allow XML Import of files with embedded DTD
* [System] Need to handle xml import when no dtd is declared