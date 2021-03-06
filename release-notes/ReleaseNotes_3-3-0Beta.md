Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.3.0Beta
June 23, 2009
----------------------------------

This is the Beta release of version 3.3.0. Owing to the extent of
new features in this release, we are eager to get feedback from
Beta testers. In particular, the following new areas of
functionality deserve attention:

Distribution Resource Planning (DRP)
  * Full spec: http://www.xtuple.org/DistributionResourcePlanning

Improved VAT and international tax support
  * Full spec: http://www.xtuple.org/EnhancedTaxInternationalization
  * Beta adds the following
	- Support for tax on Return Authorization
	- Support for tax on Credit Memo
	- Support for tax on A/R Misc Credit Memo
	- Support for tax on A/R Misc Debit Memo
	- Support for tax on Purchase Order
	- Support for tax on Voucher
	- Support for tax on A/P Misc Credit Memo
	- Support for tax on A/P Misc Debit Memo
	- New Tax History Report 

EDI Profiles Revision
  * Full spec: http://www.xtuple.org/EDIProfilesRevision
  * Beta adds support for 
	- Incidents
	- Sales Order Acknowledgements
	- Invoices
	- A/R Statements
	- Purchase Orders
  * Bcc now working
  * EDI Profiles on Customers now working

Multiple Accounting features
  * Re-allocation of AR applications
  * Automated forward-updating
  * Reverse Cash Receipts
  * Printing AR Memos
  * And more....

Translation
  * Support for translating extension packages

----------------------------------

The following features and bug fixes have been added to the applications
since the release of 3.3.0Alpha. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [Accounting] Add tax code to A/R misc. memos
* [Accounting] Allow multiple tax distributions for Misc Credit and 
Debit Memos
* [Accounting] Allow cash receipts to distinguish between distribution
date of receipt, and application date to documents
* [Accounting] Credit Card pre-authorizations create cash receipts as
"Credit Memo" not "Customer Deposit"
* [Accounting] Specify globally whether credit cards should generate
credit memos or customer deposits
* [Accounting] Add text search to Enter Order Receipt window
* [Inventory] The "To" name on the order cluster search should show the
ship to name if one exists
* [Inventory] Add right-click menu Print Receipt Label to PO Receipt
screens
* [Manufacture] Indented Work Order screen tab to edit and issue
materials
* [Manufacture] Add filter check box "Item Not In Stock� to Inventory
Availability By Work Order
* [Purchase] Tax calculation needed on PO
* [Purchase] Add tax calculations to Purchase Orders
* [Purchase] Add List Search to "Unposted Purchase Order� screen
* [Purchase] Add a list filter and vend item# column to "PO Items By
Vendor� Report
* [Purchase] Add Vendor description column to quick order entry tab
* [Sales] Enhance Tax handling - omnibus
* [Sales] Add ability for new/edit Characteristic Assignments to
Customers by Characteristic report
* [System] Global EDI profiles don't allow a way to default e-mail 
address
* [System] Add From and BCC address to EDI profiles
* [System] Add Bcc: option to EDI profiles
* [System] Password change utility
* [System] Enforce Characteristics input mask and regex validator
* [System] Add ScriptToolbox::getTempDir() method
* [System] Comment types can be associated with many different items


Bug Fixes:

* [All] Issue Stock to Shipping permission does not work alone
* [Accounting] potential issue with trigger _checkheadbeforetrigger()
* [Accounting] It is not possible to enter Start Date for General Ledger
Series
* [Accounting] Remove column options in AR Applications report
* [Accounting] Number -1 on cash receipt
* [Accounting] Tax - Item Tax Type/Tax Auth - Select Should be Most
Specific
* [Accounting] Not able to save Purchase Order Comments
* [Accounting] Privilege hole in Sales Order
* [CRM] Tab order in ToDo item entry skips "owner� and "assigned to�
* [CRM] Selecting to associate a CRM account with a customer displays
error
* [CRM] Selecting to Edit and Save an Opportunity creates a new one
* [CRM] User is able to edit "Use of Contacts� in Contact's view mode
* [Inventory] External Shipping List: User is unable to create a new
external shipping maintenance
* [Inventory] External Shipping List: Wrong window display in View mode
* [Inventory] User is able to save expense category without name and
description
* [Inventory] Ship order: Selecting "Create and Print Invoice� and
"Print Packing List� displays an error for a Job Item
* [Inventory] Posting PO Receipts requires "MaintainPurchaseOrders�
privilege but is an inventory function
* [Inventory] Slow query performance in larger databases at Shipping
* [Manufacture] Selecting to correct operations posting displays an
error
* [Products] It is possible to add Conversion, new Sites and Sources for
an Item in VIEW mode
* [Products] Selecting to create a Item cost for an Item displays error
* [Purchase] Incorrect message when printing PO
* [Purchase] Incorrect alter quantity message on a non-inventory item
 * [Purchase] Database error selecting postPoReturnCreditMemo
* [Purchase] It is possible to save Terms without specifying any code
* [Sales] Email EDI profiles on customers do not work
* [Sales] Canceling Kit Item closes all SO lines
* [Sales] Ability to comment a line item on Sales Order
* [Sales] Customer info disconnected on Sales lookup report
* [Sales] Sales History by Customer link to Invoice Information does not
work
* [Sales] Lockup/crash when opening sales order
* [Sales] User is able to create duplicate records for Sales
* [Sales] It is possible to save Sales Category without specifying name
* [Sales] Sales Representative: Selecting to associate employee doesn't
save
* [Sales] It is possible to create empty Customer groups
* [Sales] Sales history archived by error cannot be restored
* [Sales] A/R Account Assignments: User is allowed to duplicate records
* [Sales] Packing List Batch: Selecting "X� button to add SO generates DB
log error
* [Sales] Possible to have no SO orderdate on cohead
* [Sales] Error canceling Sales Order when projects are auto-created
* [Sales] User is unable to create new Prospect
* [Sales] Selecting to print a Quote generates DB log error
* [Sales] Sales order print displays blank page and generates DB log error
* [Sales] Update Prices does not update Characteristic prices
* [System] User is allowed to add/revoke privileges to a group in view mode
* [System] Grant access to only selected sites gives an error
* [System] It is not possible to save a new employee record
* [System] Error message when editing users
* [System] Mismatched variable naming in getshiptonumberfrominfo
* [System] Missing sort directive in getshiptonumberfrominfo
* [System] Issues with getshiptonumberfrominfo function

----------------------------------
Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.3.0Alpha
June 03, 2009
----------------------------------

The following features and bug fixes have been added to the applications
since the release of version 3.2.2. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [All] Add "Copy to Clip Board" to XTreeWidget default Context Menu
* [All] Application has hard-coded shortcut keys
* [All] Integrate xTuple user and PostgreSQL users
* [All] Need to determine translation mechanism for screen builder
extensions
* [All] Updated menus to be more memory efficient and to address some
issues related to rescanning privileges
* [Accounting] Add ability to filter out trial balances with no balance
or activity.
* [Accounting] Change or Remove the automatic forward account balances
capability in Accounting
* [Accounting] Add option to make forward updating accounts fully
automatic
* [Accounting] Enable reversing of Cash Receipt postings
* [Accounting] Adjustment Types description column show name value
* [Accounting] Enable re-allocation of AR applications
* [Accounting] Need to do a negative cash receipt
* [Accounting] Display Cash Receipt subtotals
* [Accounting] Preserve cash receipt info in arapply, credit memos,
and cash deposits
* [Accounting] Enhance Expense Cat Master List to Show G/L Accounts
* [Accounting] Invoice: Add Due Date and Discount Date
* [Accounting] Cannot control Customer's Check Date
* [Accounting] Reference and Notes for Vouchers
* [Accounting] Printing Debit Memos or Credit Memos
* [Accounting] Voiding vouchers does not undo distributions
* [Accounting] Change Reprint Invoices to allow selection by Balance
Due
* [Batch Manager] "Make "Submit Action to ..." Send Email
* [CRM] Add email to searchable fields on CRM Search for Contact
* [CRM] Improve visibility to prior comments on Incident Workbench
* [CRM] Need ability to edit comments
* [CRM] Create Jump To field for incident number
* [CRM] Comments for To-Do's and Tasks
* [Inventory] In Built Inventory Availablity by...
* [Inventory] ABC Classcode and Cycle Count Frequency added to
dspItemSitesByParameterList.cpp
[Inventory] Add an ability to set Location Default whilst Posting
to Inventory
* [Products] Create Item Site by Class Code Util - Needs First
Group field
* [Purchase] Purchase Order Items Window - Prices Tab
* [Purchase] Enhance PO Report Def - Alt Address Prints as Ship To
* [Schedule] Add Distribution Resource Processing (DRP) capability
to Standard Edition
* [Sales] Reorganize and consolidate customer information
* [Sales] Add button to Return Authorization workbench to create a
NEW RA
* [Sales] Rcv site in RA header doesn't affect sites in RA items
- P/R Column
* [Sales] Add Function getpacklistitemlotserialqty()
* [Sales] Explode Kits on Return Authorizations same as Sales Orders
* [Sales] Allow Kit components to inherit COS from Kit parent
* [System] Change default script extension to .js
* [System] Add support on lists (xtreewidget) for export to CSV, ODF
and HTML file formats
* [System] Expose method to add right click menu on xtreewidget and
xtreeview via scripting
* [System] Provide method to open core xTuple screens from other
screen builder screens
* [System] Rework layouts on windows using parameterGroup and
warehouseGroup to use "natural" layouts
* [System] Additional alert functionality when cost exceeds max cost
* [System] Enable incident emails by category setting
* [System] Add the ability to purge sales orders
* [System] Reason Codes assigned to documents
* [System] Add "sticky" memory to grid sorting on xtreewidget
* [System] Add DB Configuration Option to Disallow All User Logons
* [System] Add command line arguments for specifying Enhanced Auth
and SSL boolean
* [System] add include facility to scripting


Bug Fixes:

*  [All] Date Time Stamp in comment change log displays time as
12:00:00 AM
* [All] Remove Schedule Backup menu option
* [All] Obsolete macro in widgets library
* [All] some tables have user ids but should have user names
* [All] Missing return from Screen::submit()
* [Accounting] Tax liability note on G/L transactions causes G/L
series not to group properly
* [Accounting] Post zero amount invoices to aropen, simplify AR
Open query
* [Accounting] Accounting menus inconsistent
* [Accounting] possible to have a closed aropen item with no
aropen_closedate
* [Accounting] Customer Information Workbench missing previously
available information
* [Accounting] Privilege Hole in Sales Order
* [Accounting] Viewing Unposted Invoices
* [Accounting] Sales Order Lookup - Pattern Matching Not Working
* [Accounting] Inactive Vendors not controlled in miscellaneous
voucher entry
* [Accounting] Rescan privileges ignores initMenu script
* [Accounting] Right click drill down results on A/R aging are
incorrect
* [Accounting] GL Trans Report for Doc Type 'IN' does not display
Customer Name
* [Accounting] CR notes not carried forward
* [Accounting] Need to do a negative cash receipt
* [Accounting] Negative cash receipts
* [Schedule] MRP - Grouping Adds Extra Day
* [Accounting] Possible rounding errors when vouchering/processing
in multiple currencies different from base
* [Accounting] Able to save and 'post' a blank Cash Receip
* [Accounting] Deposit Registry does not total Base Balance
* [Accounting] Cash Receipts missing Base Amount column and
total
* [Accounting] Cannot load CSV credit card information to
custcreditcard view
* [Accounting] Cannot load CSV G/L Accounts from glaccount view
* [Accounting] Financial reports printing zeros by group headers
* [Accounting] Post Check generates "Check does not balance"
error message
* [Accounting] Fix Serial Columns screen Fix button produces
error
* [Accounting] Db error posting misc. check with debit memo
* [Accounting] Menu Item Tool-tips non-translatable
* [Accounting] API view glaccount incorrectly defaults profit_center
and sub_account to '1'
* [Batch Manager] creating an edi profile gives missing
ediprofile_emailhtml error
* [CRM] User is able to edit 'Use of Contacts' in Contact's
view mode
* [CRM] Special characters problem on incident workbench?
* [CRM] Tab order incorrect in Task Window
* [CRM] Can not double click opportunity
* [CRM] Contact not opening on double-click
* [CRM] Text > Integer issue
* [CRM] saveAddr() uses wrong comparison technique
* [CRM] tab order in ToDo item entry skips "owner" and "assigned
to"
* [Inventory] Detail Inv Hist by detail Date range do not
deactivate
* [Inventory] error message on delete site location is misleading
* [Inventory] Inventory UOM vs Vendor UOM on Receiving screen.
* [Inventory] Print Shipping Form screen -- Remove shipping
charges
* [Inventory] Multiple Issue Stock to Shipping cause Packing List
to report incorrect Qty Shipped
* [Inventory] Post Count Tag Difference can create multiple
entries for same location, same item
* [Inventory] Update ABC class generates DB log error
* [Inventory] Able to create blank Site type record
* [Inventory] Deleting Site type record generates DB log error
* [Inventory] Transfer Order does not expand list correctly
* [Manufacture] Return W/O Mat. Batch -- Commit executed
erroneously after error
* [Manufacture] Disassembly Work Orders Should not check Order
Parameters
* [Products] Copy BOO doesn't copy closewo flag
* [Products] Canceling to create a new item group member displays
mismatched message
* [Products] Delete does not refresh list in Class codes
* [Purchase] Purchaseorder api allows import of leading zeros
* [Purchase] Characteristics not printed on PO
* [Purchase] User is allowed to post comments while viewing
Purchase Order details
* [Purchase] Purchase Request by Planner Code does not expand
list correctly
* [Reports] Backlog by Customer mixing information
* [Reports] Financial Report Grade 0 errors
* [Reports] SO Picklist - Wrong Use of Line Function
* [Sales] Can not issue credit on credit card processor from
script
* [Sales] UPC does not show up on Item search scree
* [Sales] Credit Memo Item Search error when Item UPC Code checked
* [Sales] Update ship via on invoice and packing list when SO is
saved
* [Sales] Kits do not delete from SO
* [Sales] Negative customer discount was removed
* [Sales] Error importing to api.salesline
* [Sales] Update Prices does not update Characteristic Prices
* [Sales] Credit memo item lookup (ctrl-L) fails due to lack of
explicit type casts in PostgreSQL 8.3.X
* [Sales] Sales order contact information is missing from
api.salesorder
* [Sales] api.salesorder should allow for manually set number even
when numbering is set to automatic
* [Sales] SO and Invoice not honoring default UOM in pricing
* [Sales] SO Ship To Phone Number does not write to invchead table
* [Sales] RA Workbench: Print RA with selected customer type
generates DB log
* [Sales] Packing List Batch: Selecting "x" button to add SO
generates DB log error
* [Sales] creditCard.cpp compiler warning
* [Sales] Customer Information Workbench does not check for
privilege
* [Sales] Quote for Prospect does not filter contact list to
selected CRM account
* [Sales] Newly created invoices are not displayed in Customer
Workbench
* [Sales] Summarized Sales By Customer By Item - Average Price
Calculation is Wrong
* [Sales] Sales History by Customer link to Invoice Information
does not work
* [Sales] Selecting disposition as "Credit" and credit by as
"None" displays database error
* [System] Free floating windows don"t close when application
closes
* [System] Images list unusuable over slow remote links
* [System] locale - timestamp format issue
* [System] Change parameterGroup and warehouseGroup to layout
and size naturally
* [System] Edit User cancel button does not wor
* [System] Add command line arguments for specifying Enhanced
Auth and SSL boolean
* [System] schedule server backup or server maintenance with
time but no date gives sql error
* [System] empty default credit limit causes an error importing
sales order xml
* [System] replace OpenMFG with Manufacturing
* [System] add include facility to scripting
* [System] User is allowed to add/revoke privileges to a group
in view mode
* [System] Exchange Rates: Overlapping of date ranges generates
DB log error
* [System] api.creditmemo - cust_number Not Defaulting Bill-To
Info
* [System] Qt designer (external) gives driver errors when
opening
