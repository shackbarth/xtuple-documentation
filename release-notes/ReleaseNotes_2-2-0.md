Release Notes
xTuple Applications
OpenMFG - PostBooks
Version 2.2.0
August 23, 2007
----------------------------------

This is the final release for version 2.2.0 of OpenMFG and PostBooks.
Here are a few of the release highlights:

This is the first full release of PostBooks, the open source
Accounting, ERP, and CRM package based on the OpenMFG ERP suite.

The menu structure of the OpenMFG application has been changed from
previous releases to improve usability. The "Neo" menu structure
can be turned on and off on the User Preferences screen. This option
will be removed in a future release, as we standardize on the "Neo"
style.

The first phase of the API project implements Intelligent Database
Views to simplify importing data for Customers, Quotes, and Sales
Orders.  Voice your opinions about which views should be written
next at http://www.xtuple.org/?q=node/4299

The new inter-warehouse Transfer Order feature allows building
collections of Items to move from one warehouse to another, then
shipping and receiving those collections in the same way Sales and
Purchase Orders are handled.

The CRM module now supports Opportunity Management.

A number of screens now remember column sizes. These same windows
allow the user to select columns to show or hide and remembers which
columns have been hidden.

PLEASE NOTE: The application-based help files have not yet been
updated for the final 2.2.0 release. You can find a partially updated
version, current as of 2.2.0Beta2, on our website at the following
location: http://www.xtuple.com/docs/userguide

UPGRADE NOTES:

A number of underlying tables have been changed to support Transfer
Orders.  See the notes for 2.2.0 Beta2 below for details.

See the release notes below for details on all the new features and
bug fixes added to this release...

----------------------------------

Release Notes
xTuple Applications
OpenMFG - PostBooks
Version 2.2.0
August 23, 2007

----------------------------------

The following features and bug fixes have been added to the application
since the release of version 2.2.0-RC1:

New features:

* [System] Added new and resolved conflicting accelerator keys for menu
  items on Windows
* [A/R] Created new privileges for viewing Invoice and Deposits
  Registers
* [A/P] Added a new privilege for posting AP Checks
* [Sales] Changed the Customers By Characteristic display and report to
  find those Customers without a particular Characteristic.

Bug fixes:

* [S/O] Set the default Shipment number to a valid value if it is invalid
* [S/O] Fixed the Sales Order Item list to color-code items correctly if
  only one item is overdue
* [System] Changed OpenMFG.org Home to xTuple.org Home in the Community menu
* [I/M] Update the Transfer Order header so changes to the source warehouse
  are correctly handled by the Transfer Order Item window
* [Inventory] Hide the Perishable checkbox on the Item Site window if
  Lot/Serial functionality is disabled
* [Inventory] Hide the WIP Location checkbox on the Item Site window if
  Routings functionality is disabled
* [Products] Hide the BOO button on the Item window when creating new Items
  to avoid problems creating BOOs for non-existent Items
* [System] Rebuild menus after changing configuration settings for number
  of warehouses and Routings
* [Schedule] Do not show irrelevant items on MRP and MPS Detail displays and
  reports
* [Purchase] Add Buy Card to the Purchase menu
* [Schedule] MRP no longer creates work orders to build purchased Items which
  happen to have BOMs defined
* [CRM] Created an Opportunities report for the Print button on the window
* [Products] Changed "Make-to-Stock" label on Itemsite back to "Stock"
* [Manufacture] Fixed problem causing Post Misc Production failures in
  PostBooks
* [Sales] Fixed invalid S/O Pick List default form in the Quick Start
  database
* [A/P] Closed unprivileged access path to the Uninvoiced Receipts window
* [Inventory] Fixed problem causing the Show Allocations window to fail in
  PostBooks
* [Inventory] Fixed problem causing Cost Category updates to fail if no
  Transfer Order Liability account is set
* [Inventory] Hide Labor and Overhead Cost Category Account on Cost Category
  window if Routings functionality is disabled.
* [Inventory] Changed Running Availability window to display Purchase
  Requests in PostBooks
* [All] Fixed Print Range feature when printing reports
* [Accounting] Addressed error message when posting Invoices for Items
  without Item Sites

----------------------------------

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


----------------------------------

Release Notes
OpenMFG
Version 2.2.0Beta3
July 26, 2007
----------------------------------

This is primarily a bug fix release, but it also features new 
Opportunity Management functionality for CRM. More column 
memory functionality has been added for screens which use the 
XTreeWidget. And custom commands may now call reports stored 
in the database.

	
----------------------------------

The following features and bug fixes have been added to the application 
since the release of version 2.2.0Beta2:

New features:

* [All] Added ability to show/hide columns in displays which use the 
XTreeWidget by right-clicking on the header
* [Purchase] Added new printing and EDI capabilities when saving 
unposted and/or open Purchase Orders
* [Sales] Added additional reporting capabilities when processing Sales 
Orders, including the following: new right-click options from List Open 
Sales Orders; new print options when saving a Sales Order
* [CRM] Added Opportunity Management in CRM
* [System] Added argument to allow custom commands for RPTrender to 
point to a report in the database 
* [System] Made access to Preferences a privilege


Bug Fixes:

* [Products] Added privilege missing for post Standard Cost 
* [P/D] Fixed issue where change log items were not being recorded 
properly on the Item master
* [P/D] Fixed issue where Item master Comments were lost during 
migration
* [P/D] Made WIP Locations more legible when creating a new Work Center 
record 
* [P/D] Enabled ITEM SITE button to work on new Items 
* [P/D] Fixed issue where users viewing an Item master could edit an 
Item Site 
* [Inventory] Enabled creation of Inventory history records in transit 
Warehouses 
* [Inventory] Fixed shipform_id foreign key error when saving Transfer 
Orders
* [I/M] Enforced date requirement when doing Transfer Order Quick 
Entries
* [I/M] Fixed Transfer Order message which was referring incorrectly 
to Sales Order 
* [S/R] Added correct Doc Type for Transfer Order Freight Receipts
* [S/R] Fixed error gotten after posting Transfer Order Receipt
* [Purchase] Fixed Vendor change log to properly record changes
* [W/O] Fixed issue when Routings are disabled, the view materials 
option is disabled on the W/O Schedule by parameter and item displays
* [Sales] Fixed system error when creating a new Quote
* [Sales] Required input on Search for Sales Order by Customer P/O 
display
* [S/O] Fixed upgrade script from 2.1.1 to 2.2Beta1 to handle very 
old data
* [S/O] Fixed problem with high CPU usage when List Open
Sales Order window open
* [A/R] Fixed issue with �Find Document� field selecting multiple 
documents on Cash Receipt screen
* [A/R] Fixed TAB order on Cash Receipt screen 
* [A/R] Fixed A/R Workbench to better handle conflicting Document 
numbers
* [A/R] Fixed issue where right-click view of Credit Memo was not 
showing data on A/R Workbench
* [System] Fixed issue where two fields were not being copied when 
copying a Locale
* [System] Fixed issue in Inventory configuration where Next Transfer 
Order # was not being saved
* [System] Fixed layout of field labels on Configure Sales screen 
* [System] Fixed disabled field on Inventory Configuration screen
* [Reports] Fixed issue with Tax and total not printing on the Sales 
Order Credit Memo


PLEASE NOTE: The 2.2.0Beta2 documentation is available on our website
at the following location: http://www.xtuple.com/docs/userguide/.


----------------------------------

Release Notes
OpenMFG
Version 2.2.0Beta2
July 13, 2007
----------------------------------

This release contains several additional enhancements over the
previous. The most notable is the menu structure change, which should
be easier for users to understand and navigate. The "Neo" menu
structure can be turned ON/OFF on the User Preferences screen. This
option will be removed in a future release, as we standardize on
the "Neo" style.

The Transfer Order functionality has been expanded to include the
following:

- Shipments By Date display
- Allocations and Quantities on Hand (if the Item Site records exist
  for the destination Warehouse)
- Bar code support for Transfer Orders and Transfer Order Line Items 
  (only used on Issue To Shipping)
- The following screens have also been affected: Issue To Shipping, 
  Maintain Shipping, Recall Orders, Ship Order, Print Packing List, 
  Print Packing List By Ship-Via, Packing List Batch, Print Shipping 
  Form, Enter Order Receipt, Enter Order Item Receipt, Print Labels 
  By Order, and Unposted Order Receipts 


Also, for now, Transfer Orders only support one transit Warehouse.

Some underlying tables have been changed to support Transfer Orders:
sopack, coship, cosmisc, porecv. these have been replaced with pack,
shipitem, shiphead, and recv respectively. These new tables have
additional referential integrity constraints on them. The new tables
are populated as much as possible while still meeting the constraints
from the old tables. The old tables have been renamed
'obsolete_oldname' for reference. To allow existing reports to work,
views have been created with the same names as the old tables but
selecting from the new tables with appropriate filters (e.g. the view
sopack selects the appropriate columns from the pack table and only
rows that apply to sales orders).

Several other changes have been made to speed up and ease the process
flow on the following screens:

- Entering Discounts on the Select Payments screen
- Posting Operations screen
- Creating Credit Memos allows alternate Credit Memo value for Returns 
  on the Uninvoiced Receipts/Returns and Enter Returns screens


----------------------------------

The following features and bug fixes have been added to the application 
since the release of version 2.2.0Beta1:

New features:

* Restructured Menus
* Simplified the application of Discounts during vouchering
* Allowed the user to override the default value when creating Credit 
Memos on Returns of Purchase Orders
* Expedited Post Operations by supporting additional bar code scanning 
* Added Uninvoiced Receipts and Returns value to printed report
* Added ability to copy Item Sites
* Added the ability to disable Multiple Warehouse capability in Inventory 
Configuration if only one warehouse exists in the system.  
* Added the ability to disable Lot/Serial Control in Inventory 
Configuration if no Lot/Serial controlled items exist
* Added the ability to disable Work Order Routings in Product Configuration 
if no BOOs or Work Order Operations exist in the system
* Added the ability to disable Breeder BOMs in Products Configuration if 
none exist in the system 
* Added the ability to disable Transforms in Products Configuration if no 
transforms exist
* Added the ability to disable Buffer Management in Schedule Configuration

Bug Fixes:

* Disallowed posting Declined Credit Card Payments
* Fixed issue with Batch Manager not sending email to some SMTP servers
* Added file extension when exporting contents from right-click menus
* Vendor name is not displayed in the Vendor Address List window
* Select button on Vendor Address List is enabled even if the list is empty
* Sort order on Summary BOM report and display is inconsistent
* Save on Item window gives warning about missing Product Category when the 
first category in the combo box is selected
* Multiple-line report descriptions display improperly in the Reports window
* Misc. Charge and Freight Currency on Quote and Sales Order windows should 
be read only
* Budget window does not open correctly from Budgets window


PLEASE NOTE: The application-based help files have not been updated for
this release.

----------------------------------

Release Notes
OpenMFG
Version 2.2.0Beta1
July 3, 2007
----------------------------------

This release contains a preview (i.e., partial implementation) 
of the upcoming Inter-Warehouse Transfer Order functionality. 
You can review and test this functionality in the following 
locations:

	* I/M | Inventory Transactions
	* S/R | Issue Stock to Shipping
	* S/R | Ship Order

Also included in this first beta release of version 2.2.0 is 
the First Phase API project. This first step implements 
Intelligent Database Views for Customers, Quotes, and Sales 
Orders.

Users will also find that several screens now remember their 
column sizes, thanks to changes made to the XTreeWidget.

	
----------------------------------

The following features and bug fixes have been added to the application 
since the release of version 2.1.1:

New features:

* Expanded budgeting capability, including the ability to copy and print 
Budgets
* Added new Doc Type (CD) for identifying Customer deposits (i.e., 
unapplied Cash Receipts)
* Added column memory to screens which use the XtreeWidget; these 
screens will now remember their column size from session to session
* Added the ability to print paperwork for Returns  
* Added Print Payables Journal option to List Unposted Vouchers screen
* Added a Vendor Type filter to Vendor search lists
* Added PRINT button on Item master Images tab to allow printing of Item 
Images
* Added scroll bars to Item Image screen to allow scrolling through 
large Image files
* Added ability to view Item Images from the Item master
* Added Account column to Incident Workbench
* Removed legacy financial reports 
* Added Freight info to Receiving screen
* Added lookup button for Vendor Item Number on the Purchase Order Item
screen
* Add BOO button to Item Master screen
* Changed Incident "Notes" to "Comments"
* Updated AP Check to use Vendor Remit Address if it exists
* Added section that displays Lot/Serial Shipment information on the 
Packing List report definition
* Added privileges controlling access to the Warehouse Week and Warehouse 
Calendar Exception screens


Bug Fixes:

* Fixed Uninvoiced Receipts and Returns report definition to include 
non-Inventory Returns
* Added privilege checking to BOM button on Item master
* Improved performance when opening a new Purchase Order or converting 
a Purchase Request to a Purchase Order
* Fixed issue where changing the Ship-To Address on a Sales Order 
resulted in two new Addresses being created
* Improved messaging and options when users enter Customer numbers 
already used
* Fixed issue where viewing/editing an Invoice could incorrectly trigger 
a Tax Authority change
* Fixed issue where in rare cases A/R open records were not being created 
from posted Invoices
* Fixed A/R Aging report so it works now on PostgreSQL 8.0.X databases
* Fixed A/P Aging report so it works now on PostgreSQL 8.0.X databases
* Fixed issue where the Final Location was not being transferred when 
copying a BOO
* Modified the XtreeWidget view to stop resizing auto columns if they 
have been manually edited
* Added message Slow Moving Inventory screen if no cutoff date entered
* Fixed issue which resulted in improper error when applying A/P 
Discounts
* Fixed issue with QOH display screens re-sizing in undesirable manner
* Fixed issue where Customer defaults were not being used when Customers 
were created from CRM
* Added privileges to control access to the Maintain Budget screen
* Fixed issue with some Customer Addresses not being easily readable from 
Customer search screen
* Fixed performance when opening the Series Journal Entry screen and also 
when posting Standard Journals
* Fixed issue where Shipping Charge, Shipping Form, and Hold information 
was not being saved on Quotes
* Fixed issue leading to error when deleting a Customer
* Fixed issue with Shipments failing in scenario where the Standard Cost 
is fractions of cents
* Updated Quote report definition to correctly handle Tax changes 
introduced in OpenMFG version 2.1.0
* Fixed issue where Sales Order Line Item Tax was not being updated 
correctly when the Tax Authority on the Sales Order header was changed
* Fixed issue where Customers created from CRM could be created without 
required fields
* Fixed issue where G/L Transactions display could be erratic when if 
queried multiple times

PLEASE NOTE: The application-based help files have not been updated for
this release.


