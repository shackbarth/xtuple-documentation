Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.2.0Alpha
November 10, 2008
----------------------------------

This is the Alpha release of version 3.2.0. We are especially eager
to hear feedback from alpha testers on the following new areas of
functionality:

Freight Pricing
  * Full spec: http://wiki.xtuple.org/FreightPricing

CRM Enhancements
  * Graphical calendar view for To-Do list
  * Document Ownership
  * To-Do alarms
  * E-mail notice for Incident
  * Document links for Account and Incident

Reference Designators on BOM
  * Full spec: http://www.xtuple.org/mantis/view.php?id=7258

EDI for Checks
  * Full spec: http://www.xtuple.org/mantis/view.php?id=6909

New OpenRPT Features
  * Added crosstab object
  * Ability to print images from files on disk
  * Added zooming functionality
  * Drag selection of multiple items
  * Added group alignment tools

----------------------------------

The following features and bug fixes have been added to the applications
since the release of version 3.1.0. Additional detail for each item
listed below may be found on our community website (www.xtuple.org).
Simply go to the Issue Tracker and select the Changelog option.


New Features:

* [All] Added api.itemcost Scripts
* [Accounting] Added detail information to g/l transactions
* [Accounting] Created capability to generate ACH check files
* [Accounting] Added search capability to A/R Workbench
* [Accounting] Added running totals to G/L transaction report
* [Accounting] Added grand total to A/P Check Run Edit List
* [Accounting] Added Printed column to Unposted POs
* [Accounting] Added sort by due date to Select Payment screen
* [Accounting] Reformatted Work order operation window
* [Accounting] Added timestamp to detailed inv hist lot/serial report
* [Community] Added Link to xTuple Wiki on "Community" tab
* [CRM] Show total count on To-Do list based on selection criteria
* [CRM] Added the functionality to associate documents to an Account
* [CRM] Added File/URL links to Incident Window
* [CRM] Added Owner information to CRM that defaults to creator
* [CRM] Added priority to To-Do
* [CRM] Enabled navigation to Customer via CRM from To-Do list
* [Inventory] Added ability to review reorder point calculations before
committing updates
* [Inventory] Added "Ship Via" Column to Print Packing List Batch
* [Products] Added item sources tab to item window
* [Purchase] Added PR # to PR displays
* [Sales] Added contact to Sales Order
* [Sales] Added "Firm" status to Sales Order Lines:
* [Sales] Added api.creditmemo and creditmemoitem views
* [Sales] Added ability to define shipping and receiving warehouse on
Return header
* [Sales] Added toggle button to Sales Order screen to allow for simpler
presentation
* [Sales] Included baseline sales order acknowledgment form
* [Sales] Added Cust. info to S/A displays/reports
* [Sales] Updated customer screen
* [Sales] Added Advanced freight calculation functionality extension to
xTuple ERP
* [Sales] Added the ability to mass update prices by amount
* [Schedule] Made firm Planned Orders different color
* [Schedule] Added API view for Planned Order
* [Schedule] Created API view for Purchase Orders
* [Schedule] Added check box option on Item Site screen next to Lead
Time that allows you to "Use on first grouping"
* [System] Converted all embedded mql files to use new database driven
metasql queries
* [System] Converted XMainWindows and XDialog Windows to XWidget


Bug Fixes:

* [All] Fixed compile errors on OpenSolaris
* [All] Fixed startOfTime() and endOfTime() stored procedures which
weren't working with some PostgreSQL datestyle settings
* [Accounting] Fixed blank description column on To-Do/Incident
* [Accounting] Fixed issue with Cash Receipts report ignoring selection
criteria
* [Accounting] Fixed refresh on AR workbench
* [Accounting] Fixed api.invoice insert error where CASE types text
and integer could not be matche
* [Accounting] Fixed issue with run time reporting to G/L regardless
of selection in BOO
* [Accounting] Disallowed single voucher from appearing on multiple
checks
* [Accounting] Fixed mixed mode problem when jumping to CRM account
from Tax Authority Window
* [CRM] Fixed empty window found when selecting to edit the �Uses of
the Contact� in contact screen
* [CRM] Fixed issue preventing selection of open windows when opened
through To Do List
* [Inventory] Fixed issue where Now and Today's date were not treated
the same on Where Used display
* [Inventory] Fixed issue preventing relocation of stock when a
Location is non-netable
* [Inventory] Fixed issue where non-netable location remained netable
if checked after stock received into it
* [Inventory] Reinstated version of report that shows graph
* [Inventory] Fixed itemsite api view to allow update of inactive
Item Sites
* [Inventory] Fixed issue where external shipping maintenance screen
opened behind desktop
* [Products] Made detailed item costs display revision-aware
* [Purchase] Fixed crash behavior on Post PO by Agent screen
* [Reports] Fixed Invoice report, which was printing blank total detail
* [Reports] Clarified wording of html email label
* [Sales] Fixed non-functional bill-to phone number on S/O
* [Sales] Fixed non-functional pattern in RA Workbench
* [Sales] Fixed blank type column on Invoice Information screen
* [Sales] Ensured City, State, and Zip information are displayed when
adding new Ship-To address
* [Sales] Required List Unposted Credit Memos screen include C/M's with
no line items
* [Sales] Removed closed Invoices from displaying on Customer
Information Workbench
* [System] Fixed problem with numeric sort order not working as expected
* [System] Removed superfluous user preferences
