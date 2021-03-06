Release Notes
xTuple Applications
OpenMFG - PostBooks
Version 2.2.0RC1
August 15, 2007
----------------------------------

This is the first Release Candidate for version 2.2.0 of OpenMFG and
PostBooks. This is primarily a bug fix release, improving on issues 
discovered by the community during testing of 2.2.0Beta3.

	
----------------------------------

The following features and bug fixes have been added to the application 
since the release of version 2.2.0Beta3:

New features:

* [Inventory] Added default Cost Category definition to Transit 
Warehouse master to help with handling auto-created Item Sites
* [Inventory] Updated Transfer Order (T/O) logic so that automatically 
created Item Sites for transit Warehouses should have Location control 
disabled by default
* [P/O] Added $ amount to Uninvoiced Receipts and Returns screen
* [P/O] Added functionality to automatically clear received qty having 
$0 P/O Liability when marking as invoiced on Uninvoiced Receipts/Returns 
screen

Bug Fixes:

* [Products] Changed Item cost logic to only list labor and overhead 
costs when Routings are globally enabled. 
* [P/D] Fixed loophole in Mass Replace Component Item utility which 
could allow recursive BOMs
* [Inventory] Fixed Print Packing List lookup to filter for T/Os more 
effectively 
* [Inventory] Fixed error when returning stock from right-click menu 
on T/O Line Items tab  
* [Inventory] Fixed error preventing use of T/O Quick Entry screen
* [Inventory] Fixed issue with Shipping Form not working properly for 
transit Warehouses
* [Inventory] Added T/Os to views from Inventory Availability displays
* [Inventory] Fixed issue where T/Os were not being considered by 
Running Availability 
* [Inventory] Fixed issue preventing links between Warehouse Zones 
and Locations when creating a new Location
* [Inventory] Fixed issue where the T/O Freight amount only considered 
the freight value for the first T/O line
* [Inventory] Fixed issue where the application froze when using the 
"Receive Immediately" option for T/Os on the Ship Order screen
* [I/M] Fixed issues related to T/O Events not firing as expected 
* [I/M] Added T/O allocations to Item allocations logic (i.e., when 
viewed from the Inventory Availability screens 
* [I/M] Fixed issue with screen freezing after using ISSUE STOCK TO 
SHIPPING button on the List Transfer Orders screen
* [I/M] Fixed issue with  T/O Line Item Comments being unaccessible
* [S/R] Enforced assignment of "None" Control Method for Outside 
Process Items
* [S/R] Fixed possible Currency discrepancy between Freight amount 
entered on Ship Order screen and corresponding Invoice
* [M/S] Fixed MPS to not generate Planned Orders for Items having no 
assigned planning system
* [Purchase] Added configuration option to enable/disable new printing 
options when saving a P/O
* [Purchase] Fixed issue with "Show Unvouchered" option not working on 
List Unposted P/Os 
* [Purchase] Made "Vend. Item Number" and "Vendor Description" read-only 
on P/O item screen
* [Purchase] Fixed tohead error received when right-clicking on data in 
the Running Availability screen
* [Purchase] Fixed issue where closing the client before saving a Voucher 
can lead to problems 
* [P/O] Enabled ability to correct Receiving for Non-Inventory Items 
* [P/O] Fixed issue where free-form Vendor part descriptions were not being 
saved correctly
* [P/O] Fixed error received when marking as invoiced a P/O Receipt having 
$0 value from Uninvoiced Receipt/Returns screen
* [Manufacture] Disabled unneeded controls visible in Manufacture 
Configuration when Routings are turned off
* [Manufacture] Switched Order of MRP and MPS on Menu Tree in Neo menu
* [W/O] Fixed Misc Production posting to handle overhead correctly 
* [W/O] Fixed issue where the W/O Material Requirements by Component Item 
screen displayed components for closed W/Os
* [W/O] Fixed issue where correcting Operation posting didn't update the 
wooper_post table
* [CRM] Added Opportunities to Standard menu 
* [Sales] Fixed issue where line item detail was not printing in the 
standard Invoice report definition
* [Sales] Added configuration option to enable/disable new printing options 
when saving an S/O 
* [Sales] Fixed Customer Information Workbench to show accurate backlog 
information
* [Sales] Fixed "ediform" error encountered with opening the Ship-To 
screen 
* [Sales] Fixed issue with Sales Order line items not retaining Tax 
information overrides 
* [Sales] Fixed issue where it was possible to delete closed
Work Orders from the open Sales Orders which created them
* [S/O] Fixed ASAP schedule dates option on S/O configuration to work 
correctly
* [A/P] Fixed the Voucher item screen to correctly save the Tagged Yes/No 
value
* [A/R] Fixed error when attempting to edit a Cash Deposit (CD) from the 
A/R Workbench screen
* [A/R] Prevented posting Cash Deposits having no A/R Account Assignment
* [G/L] Fixed View Financial Reports screen to exhibit the same roll-up 
behavior for all report types, not just Ad Hoc
* [System] Made names consistent when right-clicking on tool icons in 
the Neo menu
* [System] Fixed error received when trying to save Inventory 
Configuration
* [System] Improved layout of Configure Inventory screen
* [Reports] Added report definition for T/O List 
* [Reports] Fixed report rendering engine to eliminate redundant query 
calls 
* [Batch Manager] Fixed issue with P/Os printing blank if scheduled 
for email delivery 

* [All] Fixed displays of Currency values to show blanks for the base 
Currency instead of "????" when the foreign value is blank.

PLEASE NOTE: The 2.2.0Beta2 documentation is available on our website
at the following location: http://www.xtuple.com/docs/userguide/.


