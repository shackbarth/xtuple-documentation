Release Notes
xTuple ERP
Version 4.1.0Beta
May 14, 2013
----------------------------------

This is the beta release of version 4.1.0. This release features
the brand new automatic update capability for the xTuple Desktop 
client. As always, we welcome feedback from beta testers. But 
please do not use beta software in production.

Information about compatibility issues related to this software
version can be found on the xTuple Compatibility Matrix at the 
following address: www.xtuple.org/compatibility-matrix.

----------------------------------

The following features and bug fixes have been added to the
applications since 4.0.3. Additional detail for each item listed 
below may be found on our community website under the Issue 
Tracker.

New Features:

* Make updates more automatic	[5837]
* Substitute items on a sales order	[19354]
* New API for entering Physical Inventory Counts [19388]

Bug Fixes:

* Freight amount is calculated incorrectly for a sales order with 
multiple shipments [17525]
* Postbooks Demo: Selecting to purge invoices generates DB log 
error [17779]
* Selecting to post a cash receipt displays a system message 
[18623]
* DB log error is generated on selecting to query "Update 
Reorder Level by Item" screen [18678]
* Irrelavent behaviour is observed in "User Information" screen 
[18705]
* Observation: Incorrect Net unit price is populated in Purchase 
Order item screen [18755]
* DB log error is generated on selecting to query the "Return 
Authorization Workbench" screen [18934]
* Irrelevent dialog is displayed on selecting to print Sale 
Types [18975]
* Unable to print "Contracts" screen [18995]
* API item view missing fields [19317]
* API requires custinfo_shipform in order to display data [19339]
* Only Show Shortages [19421]
* Trial Balance Out of Balance [19583]
* Item "Maximum Desired Cost" value not converted to local 
currency when comparing to PO Unit Price [19600]
* "purgeSalesOrders" does not exist on login after 38xto400 std 
update [19602]
* It is not possible to copy an already copied Locale [19618]
* DB log error is generated on selecting to print a Sales Order 
created for a foreign customer [19639]
* api.itemsourceprice does not include newly added public.itemsrcp 
columns [19651]
* Profit Margin doesn't recalculate [19694]
* Convert Quote to Order/Convert Quote to Invoice [19728]
* Substitute items salesOrderItem Screen [19729]
* List cost does not show in local currency [19756]
* Performance issue with Master Schedule display after migrating 
to 3.8.4 and new cloud [19961]
* View public.usr, locales, roundqty() affect performance of 
cloud db's with more users [19971]
* Return Authorization automatic numbering problem [20013]