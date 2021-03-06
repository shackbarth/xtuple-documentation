Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.5.0Beta2
March 3, 2010
----------------------------------

This is the second beta release in the 3.5.0 release cycle. If
you've been following our community site, you know our haxTuple
bug derby is well under way, with several community members
currently vying for the top prizes. If you have not registered
yet for haxTuple, there's still time to get involved. The contest
runs from February 15th to March 8th. Learn more about the rules
and the prizes being offered here: http://www.xtuple.org/haxtuple-2010

Of course, you don't have to be a developer to get involved.
We are also looking for feedback from community beta testers. So
load up your sandboxes and test away! NOTE: If you are testing
the Manufacturing Edition, the upgrade from 3.5.0Alpha to
3.5.0Beta does not require an upgrade script for the xtmfg
package--only the std350alphato350beta.gz script is required.

Sure to be of interest to everyone are the new enhancements to
the virtual (search) cluster. Beginning with 3.5.0Beta, users
will find auto-complete functionality in lookup fields
throughout the applications. Legacy lookup buttons will still be
supported. But auto-recognition of partially-entered strings
is now supported.

In this release look for the debut of the new "Parameter Widget" in
the To-Do List and Incident Workbench windows. This new widget
allows programmers to define unlimited possible filter criteria on a
report as list of parameter types (i.e. CRM Account, Contact Name,
Start Date, User Name) rather than as a fixed collection of widgets
laid out on the screen as we have traditionally done. Users can then
dynamically select from this list and build filter combination
criteria to apply to their query which they can save for future use.
Expect to see this methodology deployed throughout the application in
future releases.

Here is a list of new features to check out in 3.5.0:

Drop Ship Purchasing
  * Full spec: http://www.xtuple.org/node/2481

Expanded Pricing Effectivity Support
  * More info: http://www.xtuple.org/issuetracker/view.php?id=9603

Embedded MetaSQL Editor
  * More info: http://www.xtuple.org/issuetracker/view.php?id=7732

Tooling Management
  * Full spec: http://www.xtuple.org/node/2197

Also of note:
  * Automatic A/R Discounts
  * Improved Lot/Serial Support
  * Support for Postgres 8.4
----------------------------------
The following features and bug fixes have been added to the
applications since the release of 3.5.0Beta. Additional detail
for each item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
"Changelog" option.


New Features:

* [Accounting] Add "Post All" button to Checks tab on AP Workbench
* [Architectural] Expose OpenRPT option to pass printer to scripting
* [CRM] Add advanced incident workbench features to the core
* [CRM] Contact cluster should behave like other search clusters
* [CRM] Show total hours and expenses on Project header
* [Products] Enable DELETE BOM Item
* [Purchase] Add support for drop ship to purchase orders
* [Sales] Port Issue 9987 to core: Enhance changelog tracking for changes to a customer's ship-to's
* [System] Complete the XML Export functionality

Bug Fixes:

* [Accounting] Sales rep number requires employee name (or code) not his/her number
* [Accounting] Zero balance option should disable when single account selected
* [Accounting] Add show unposted option to AR workbench
* [Accounting] Post Invoice After Printing generates warning message
* [Accounting] Find on Script Editor says text not found even when it is
* [Accounting] Posting of cash receipt with discount does not use new discount G/L account
* [Accounting] Creating a Credit Memo from a Return do not complete account cycle
* [Accounting] Address clusters on invoice window are misaligned on Mac
* [Accounting] ACH does not work in commercial editions without batch manager
* [Accounting] Add query button to maintain shipping window
* [Accounting] Acceptance of Posting an A/P Credit Memo without a Vendor Code
* [Accounting] It is possible to create incomplete JE when canceling series entries
* [Accounting] Credit memo on vendor history is added to total
* [Accounting] Manufacturers List on Item Source Mfg ta
* [Accounting] API view api.glaccount gives error when updating
* [Accounting] Tax codes do not allow negative tax rates
* [Accounting] Summarized sales history ignored by privilege
* [Accounting] can't click on vendor widget in Misc. Voucher screen
* [Accounting] Contact information is "squished" on Mac
* [Accounting] Selecting to edit a cash receipt displays 'No Bank Account' dialog
* [Accounting] Strange behavior when reversing a reversal entry
* [Accounting] Trial balance query have unneeded transaction
* [Accounting] Invoice reprint displays wrong total after certain application
* [Accounting] Tab order Series G/L Journal Entry
* [Accounting] Sales tax credit double credits a/
* [Accounting] Post credit memo doubles tax on freigh
* [Accounting] Duplicate tax rate possible for tax code
* [Accounting] Bill of Operations: Final Location field is very narrow
* [Accounting] crash when creating a wo not designated as "site can manufacture"
* [Accounting] Posting Operations from Work Order window does not populate the W/O number
* [Accounting] Credit Memo does not display correctly from GL Transactions
* [Accounting] Cash Receipt Journal does NOT print
* [Accounting] Invoice does not recalculate tax when tax zone is changed
* [Accounting] Australian ABA file generation function for Electronic Checking formatABAChecks
* [Accounting] "Total" field on Invoice doesn't have comma formatting
* [Accounting] voucheringeditlist view is faulty
* [Accounting] Taxes are generated when they shouldn't be
* [Accounting] PreAuth to Charged Credit Cards cause Unbalanced Bank Reconciliation
* [Accounting] move ACH functionality in A/P to PostBooks
* [Accounting] Can not apply credit memos in A/R workbench
* [Architectural] Work center cluster does not auto complete
* [Architectural] Packages -> Load does not check correct location for Updater
* [Architectural] Short cut keys don't open Alias search on item cluster
* [CRM] Opportunity Tab on CRM Account has extra clutter
* [CRM] Error using pattern search in Opportunity screen
* [CRM] Show balance of Hours and Expense budgeted as columns on Project Task tab
* [CRM] It is possible to edit Characteristics in View mode
* [CRM] Tab Order incorrect when adding Primary and New Contacts from CRM Account
* [CRM] Detaching a contact and saving generates DB error
* [CRM] Contact details are not saved
* [CRM] UsernameCluster or CRMAcctCluster do not emit signals until focus is lost
* [CRM] Contact cluster duplicate check returns too many results
* [Documentation] Unable to prove statement on opening closed line on PO
* [Documentation] Docs refer to shopfloor workbench in postbooks
* [Inventory] 'Selected' option is not disabled if 'pattern' option is selected in detailed inventory history screen
* [Inventory] Performance slow on print packing list by ship via
* [Inventory] Missing ship vias in print packing list by ship vias
* [Inventory] Item availability workbench screen is visible even after revoking 'View Item Availability Workbench' privilege
* [Inventory] Sales Reservations are not reverted back if an item issued to shipping is returned
* [Inventory] Selecting to edit order from 'Total' label displays error message and generates DB log
* [Inventory] Order cluster generates sql error on search
* [Inventory] Unable to post the receipt of an expense item
* [Inventory] Editing a posted count slip quantity does not update Count tag Count Qty
* [Inventory] Cannot Ship TO Item that has already been received
* [Inventory] Selecting to summarize transaction history generates DB log error
* [Inventory] Enter Order Receipts screen displays 'O' instead of the PO Number
* [Inventory] Selecting to Reassign Lot/serial Item displays error message
* [Inventory] Can't recall partial transfer order shipment
* [Inventory] Error shipping transfer order
* [Inventory] Maintain Shipping Takes Over 5 minutes to load
* [Inventory] Transfer Orders - location detail on history
* [Inventory] New item sites default to average costed
* [Inventory] Selecting to Relocate Inventory displays error message
* [Inventory] Error when opening item site in PostBooks
* [Inventory] 'Issue Line Bal' to the items of a released transfer order, displays error
* [Inventory] Selecting to post Misc Inventory Count displays error message
* [Inventory] Selecting to create an item site for a newly created kit item generates DB log
* [Inventory] Marking Expense Categories as Inactive is not honore
* [Inventory] Can't delete any item sit
* [Inventory] DB Error on itemsite Delete in postbooks
* [Inventory] Shipping Hold Type not displayed
* [Manufacture] postproduction function does not handle backflush of operations correctly
* [Manufacture] Manufacture->Transaction->Scrap does not work for controlled finished items
* [Manufacture] Cannot Add Operations in Work Order Screen
* [Manufacture] Add Date to Close Work Order
* [Manufacture] Job Cost Items
* [Manufacture] Job Costing Report
* [Manufacture] Response to dialog is opposite selection
* [Manufacture] Tab order incorrect on Work Order Material Requirement screen
* [Manufacture] Error dialog on correct operation posting
* [Manufacture] Print Traveler button behavior on Create Work Order
* [Manufacture] Print report of Material Usage Variance by BOM item doesn't display item details
* [Manufacture] Problems with post operations screen
* [Manufacture] Close work order window doesn't go away after closing w
* [Manufacture] dspWoOperationsByWorkCenter.ui does not select WO on right-click menu
* [Manufacture] Post and correct operations screen is displayed on clicking "OK" button in the warning
* [Manufacture] Cannot post operations from work order right-click
* [Manufacture] post operation after wo closed
* [Manufacture] Posting Operation time
* [Manufacture] "Split" Items to backflush BOM and BOO upon Issue to Shipping
* [Manufacture] Inconsitencies with correct operations
* [Manufacture] Unable to return product on a work order
* [Manufacture] Deleting Materials from Work Order
* [Manufacture] Selecting to correct operation posting displays an error
* [Manufacture] dspWoOperationBufrStsByWorkCenter.ui:View or Edit operation doesn't populate work order number
* [Manufacture] Work Order indented screen Materials not sorted
* [Products] Unable to create a kit item site record
* [Products] xtmfg.schema is not referencing xmfg
* [Products] Expired BOM Component causing a recursive BOM error -- no way to get around
* [Products] Can not delete items
* [Products] Typo on texts in print report of single level where used
* [Products] Print report of costed indented BOM displays an irrelevant 'Total Cost' field
* [Products] View mode of an item enables the user to edit BOM,BOO and customer workbench
* [Products] Can not add item sites when creating a new item
* [Products] Boohead not inserting for BOO's created in previous versions
* [Products] Cannot thaw avg cost item after erro
* [Products] 'Type' field of planning item is displayed incorrectly
* [Products] Incorrect Expiry dates after mass expire are displayed in BOM
* [Products] Selecting to Mass Replace an item displays error message
* [Products] Selecting to print pending BOM changes generates DB log error
* [Purchase] Selecting to reopen a purchase order unchecks the 'Drop Ship' option
* [Purchase] Bold cursor in PO field if method is manual
* [Purchase] Saving a purchase order doesn't reset the 'subtotal' field
* [Purchase] Vendor Delete does not give user a second chance
* [Purchase] Make the vendor currency read only on item source
* [Purchase] Username on purchase orders defaults to login name not proper name
* [Reports] Invoice Report does not display Total Due when no tax is applied
* [Reports] Submitted report of Credit Memo is empty
* [Sales] Column header on Sales Report displays S/O # and should have CM as well
* [Sales] 'Selected customer' option is not disabled if 'customer ship-to' option is selected in Allocate Reservations screen
* [Sales] Choosing [caluclated freight] or [manual freight] on sales order doesn't update sales order
* [Sales] Cannot reprint cc receipt
* [Sales] Change Post Billing Selections to Create Invoice
* [Sales] Sales account assignments / Sales categories
* [Sales] cannot delete a line item after stock has been issued and returned from shipping
* [Sales] GUI issue with historical sales order view with inactive rep's name no longer appearing.
* [Sales] Deleting a Shipping Charge type creates errors
* [Sales] Customer WB not refreshing properly when changing between customers
* [Sales] Creating a new Contact from the SO New Customer option generates Error
* [Sales] Contact search screen opens out of reach
* [Sales] Table cohist does not populate cohist_ordernumber on consolidated invoice entries
* [Sales] Converting Sales Order from Quote
* [Sales] It is possible to edit prospect in view mod
* [Sales] 'Print' button is always disabled in print RA form
* [Sales] Selecting to purge invoices generates DB log error
* [Sales] Set default cursor focus to Customer Number Field on Customer Info Workbench
* [Sales] Pricing and items on sales report does not reflect the change of a customer in a sales order
* [Sales] Duplicated tax when processing a paymen
* [Sales] Sales credit allocation does not work correctly
* [Schedule] Create Planned Order defaults to Work Order not item type
* [Schedule] Planned Order comments not Displayed
* [Schedule] Enforce no multi-level MRP on planner codes in STD Edition
* [Schedule] Standard DB Version throws error whr "Run MRP by Planner" is used
* [Schedule] Time phase production by item report do not honor selected warehouse
* [System] Config Modules / Accounting - toggle "Require Vendor Invoice #"
* [System] Edit Comment of Type Genera
* [System] Fix serial columns screen accessed by non-admin user
* [System] Hide Shift from Employee Screen
* [System] there is no StatesMasterList report
* [System] User association with the employee is not indicated
* [System] MetaSQL Window has no icons on button
* [System] Allow a custom QValidator to be created with script
* [System] Eternal Light Bulb due to bad metasql

----------------------------------
Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.5.0Beta
February 12, 2010
----------------------------------

This is the first beta release in the 3.5.0 release cycle. Anyone
who has not registered yet for haxTuple (our 2d annual bug
derby), there's still time to get involved. The contest runs from
February 15th to March 8th. Learn more about the rules and the
prizes being offered here: http://www.xtuple.org/haxtuple-2010

Of course, you don't have to be a developer to get involved.
We are also looking for feedback from community beta testers. So
load up your sandboxes and test away! NOTE: If you are testing
the Manufacturing Edition, the upgrade from 3.5.0Alpha to
3.5.0Beta does not require an upgrade script for the xtmfg
package--only the std350alphato350beta.gz script is required.

Sure to be of interest to everyone are the new enhancements to
the virtual (search) cluster. Beginning with 3.5.0Beta, users
will find auto-complete functionality in lookup fields
throughout the applications. Legacy lookup buttons will still be
supported. But auto-recognition of partially-entered strings
is now supported.

Also, the new Drop Ship Purchasing features are now available for
testing in 3.5.0Beta. To learn more, see the full Drop Ship
Purchasing spec here: http://www.xtuple.org/node/2481

And don't forget to check out and test the new features
introduced in the alpha:

Expanded Pricing Effectivity Support
  * More info: http://www.xtuple.org/issuetracker/view.php?id=9603

Embedded MetaSQL Editor
  * More info: http://www.xtuple.org/issuetracker/view.php?id=7732

Tooling Management
  * Full spec: http://www.xtuple.org/node/2197

Also of note:
  * Automatic A/R Discounts
  * Improved Lot/Serial Support
  * Support for Postgres 8.4

----------------------------------

The following features and bug fixes have been added to the
applications since the release of 3.5.0Alpha. Additional detail
for each item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
"Changelog" option.


New Features:

* [Accounting] Add List Open Vouchers tab to AP workbench
* [Architectural] Enhancements to virtual (search) cluster
* [Architectural] Subclass item cluster from virtual cluster
* [CRM] Add recurring capability to activities in CRM
* [Inventory] Allow purchase receipts by bar code
* [Inventory] Avoid receive Transfer Order lines if has not been
shipped
* [Inventory] Inventory distribution should present list of
existing lots for lot-controlled items being adjusted in

Bug Fixes:

* [All] Cannot highlight by dragging across text in Item Number
field
* [All] xLineEdit copy always copies everything
* [Accounting] AR open items do not show up on screen
* [Accounting] Apply cash with discount rounding problem in
function
* [Architectural] User cluster loses user information when user
inactivated or deleted
* [Inventory] Average costing should use average cost on physical
counts
* [Sales] Returns don't properly handle Job Costed items
* [System] Updater fails to load Metasql with error after new
Metasql trigger implemented

----------------------------------

Release Notes
xTuple ERP
PostBooks, Standard, and Manufacturing Editions
Version 3.5.0Alpha
January 29, 2010
----------------------------------

This is the alpha release of version 3.5.0. This release is
packed with lots of new features, and more still to come in the
next stage of the release cycle. As always, we are looking for
feedback from alpha testers. But testers please note: the
purchasing module should be avoided, since extensive changes to
support drop shipping are not yet complete.

Here's an overview of new features in this release:

Expanded Pricing Effectivity Support
  * More info: http://www.xtuple.org/issuetracker/view.php?id=9603

Embedded MetaSQL Editor
  * More info: http://www.xtuple.org/issuetracker/view.php?id=7732

Tooling Management
  * Full spec: http://www.xtuple.org/node/2197

Also of note:
  * Automatic A/R Discounts
  * Improved Lot/Serial Support
  * Support for Postgres 8.4

----------------------------------

The following features and bug fixes have been added to the
applications since the release of 3.4.0. Additional detail for each
item listed below may be found on our community website
(www.xtuple.org). Simply go to the Issue Tracker and select the
"Changelog" option.


New Features:

* [Accounting] Reconcile Bank Accounts by Credit Card
* [Accounting] Add support for A/R discounts to Cash Receipt
* [Accounting] Add the ability to select by customer group in to
the A/R aging display and the printed report
* [Accounting] Add pricing effectivity options to sales order
* [Accounting] Selection hold button on Payables Workbenc
* [Accounting] Provide color emphasis on credit type columns on
Open Receivables display
* [Accounting] "Apply line bal." button within the "Apply A/R
Credit Memo" screen
* [Accounting] Tooling issue and return
* [Accounting] Calculate freight on Returns using freight
pricing schedules
* [Accounting] The ship order window should use the freight
calculation algorithm
* [Accounting] Add radio buttons to the Print Packlist Form
window to explicitly choose whether to print Picklist
* [Accounting] Bank rec history label should refer to date
range
* [Architectural] Embed MetaSQL editor into xTuple ERP
application and add some enhancements
* [Architectural] Adding index on arapply to improve
performance
* [Architectural] Added First Group field to api.itemsite vie
* [Architectural] Capture and log qWarning/qDebug output to
window accessible from application
* [Architectural] Remove dependency on curl for credit card
processing
* [CRM] Prompt "are you sure" when deleting a Contact
* [Inventory] Serialized Job Items
* [Inventory] Automatically generate Serial Numbers
* [Inventory] Preserve lot # during Inter-Warehouse Transfer
* [Inventory] Ability to add back into inventory previously
scrapped or expensed items
* [Inventory] Auto populate Lot/Serial
* [Manufacture] Add the ability to set W/O item cost recognition
defaults at the item site level
* [Purchase] Increase price precision
* [Purchase] Add a notes field to voucher distributions
* [Sales] Move sales order reschedule feature to the Sales Order
Window
* [Sales] Price Schedule enhancement pack
* [Sales] Add option to recalculate pricing on a sales order
when the shipto is changed
* [Sales] Add "Scheduled Date Range" criteria to the Print
Packing List by Ship Via window
* [Sales] Remove freight charge on Back Order Invoices
* [System] Rename user "groups" to "roles"; add column to List
Users

Bug Fixes:

* [All] Idle timeout does not roll back partial transactions
* [All] Blocks on db when certain screens are open
* [All] Distribution screen holds Postgres
* [Accounting] Return work order material revalues WIP
incorrectly on average cost
* [Accounting] Return Stock to Shipping for Lot/Serial MLC
items can miss distribution history
* [Accounting] reloading some api view definitions gives sql
errors on tax fields
* [Accounting] List Price UOM on item master is misleading
* [Architectural] Type setting of the XComboBox not being set
correctly to type "Adhoc"
* [Batch Manager] Update buffers status by planner code returns
query error
* [CRM] Sticky options not remembering settings
* [CRM] Cannot Delete CRM Account w/ Primary and/or Secondary
Contacts
* [CRM] when you detach a Primary/Secondary Contact from a CRM
Account, it's still there
* [Inventory] Only one item site for any item may ship at any
time
* [Inventory] Incomplete Lot/Serial transaction leaves orphaned
itemlocdist entries
* [Manufacture] Standard Operation data not available when
adding operations
* [Manufacture] BOO Instructions not in display
* [Products] Qty Per limits to Qty decimal precision on BOM
item
* [Sales] Deleting sales orders and SO line items slow
* [Sales] Performance issue with Sales -> List Quotes
* [Sales] Tax and freight not displayed in Billing Edit list
* [Sales] System Hangs on Credit Memo Line Item when item
number entered (after turning items to Exclusive)
* [System] Maintaining others preferences
* [System] XML import automatically prepends api. to all views
