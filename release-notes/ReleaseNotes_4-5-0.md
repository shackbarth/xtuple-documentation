Release Notes
xTuple ERP
Version 4.5.0 Final
June 9, 2014
----------------------------------

These are the release notes for the 4.5.0 Final Release. Thanks
to all who contributed to make this release possible. 

With the release of 4.5.0, we continue the process of revising the
naming conventions and the behavior of our core updater packages.
Our overall goal is to simplify the process of installing and
upgrading xTuple ERP databases.

Just as was true for the 4.4.1 release, you will only need to apply
one updater package to upgrade to 4.5.0--that is, assuming you are
already running on at least 4.4.0. The new updater packages are
designed to bring you all the way up to their version, no matter 
what version (>= 4.4.0!) that you're on.

In 4.5.0 we've gone a step further: not only will a single package take
you through every *version* of the app, it will also install all the
constituent parts of your edition. Before now, if you wanted to do an
upgrade to the Manufacturing Edition, you would have needed to perform 
the standard/dist upgrade and then the manufacturing upgrade. Not any
more. With the new process, only one upgrade package is needed for the
entire upgrade. No more upgrading the core and then upgrading the
related packages. Everything is upgraded all at once.

NOTE FOR DISTRIBUTION EDITION CUSTOMERS: The xwd package no longer 
exists as a separate entity. All the functionality that was contained 
in the xwd package is now included in the single "distribution" upgrade 
or install package.

To be verbose about all of this:

postbooks-upgrade-450.gz will:
upgrade a PostBooks database from anywhere >= 4.4.0 to 4.5.0

manufacturing-upgrade-450.gz will:
upgrade the standard/dist (i.e., inventory code) to 4.5.0
upgrade the manufacturing code to 4.5.0

manufacturing-install-450.gz will:
do a one-time install of tables, etc. for standard (i.e., inventory code) at 4.5.0
upgrade the standard/dist (i.e., inventory code) to 4.5.0
do a one-time install of tables, etc. for manufacturing at 4.5.0
upgrade the manufacturing code to 4.5.0

distribution-upgrade-450.gz will:
upgrade the standard/ist (i.e., inventory code) to 4.5.0
upgrade the distribution (i.e., xwd code) to 4.5.0

distribution-install-450.gz will:
do a one-time install of tables, etc. for standard (i.e., inventory code) at 4.5.0
upgrade the standard/dist (i.e., inventory code) to 4.5.0
do a one-time install of tables etc for distribution at 4.5.0
upgrade the distribution (i.e., xwd code) to 4.5.0

PLEASE NOTE: Other packages, such as Advanced Commissions and Fixed 
Assets, are currently remaining on their own release schedule and should 
be installed as before. 

To ensure compatibility, please review the xTuple Compatibility 
Matrix before upgrading: http://www.xtuple.org/compatibility-matrix.

----------------------------------

The following bug fixes have been added to the applications since the 
4.5.0 Beta release. Additional detail for each item listed below may be 
found on our community website (www.xtuple.org).

Bug Fixes:

* Privilege problem [21726]
* Work order time clock issues when spanning over midnight [22132]
* 4.1 voucher screen [22832]
* 4.3 mfg workbench error [22882]
* Omnibus fixes to business object name changes [23123]
* Only one year history [23150]
* Performance is severly hindered by linear seach of location table 
[23162]
* Inventory Availablity by Work Order in indented mode is pulling in 
irrelevant order information [23166]
* Project Type filter not working in desktop client [23223]
* Unbalanced item site after thawing non-netable count tag [23507]
* Orphaned child work orders [23532]
* PO from Sales Order not working correctly [23593]
* Item Availability WB - pop-up at open [23615]
* Information lost when converting Quote to Sales-Order [23628]
* Time and Attendence [23629]
* Sales Order Margin Detail Issues [23666]
* Time In and Time Out columns are not populated [23757]
* Margin % for Kits not displaying correctly [23758]
* Auto clock out not working [23766]
* Reschedule required on sales order item before save [23783]
* "Get G/L Distribution Date" dailog is not displayed on selecting to 
post a cash receipt from Receivables Workbench screen [23800]
* taxpay_id not serial type [23825]
* Watermarks not functioning properly in 4.4 [23555]
* Page setup off on all reports [22991]

----------------------------------
Release Notes
xTuple ERP
Version 4.5.0 Beta
May 29, 2014
----------------------------------

These are the release notes for the 4.5.0 Beta Release. Thanks
to all who contributed to make this release possible. As always, 
we welcome feedback from beta testers, but please do not use beta 
software in production.

To ensure compatibility, please review the xTuple Compatibility 
Matrix before upgrading: http://www.xtuple.org/compatibility-matrix.

----------------------------------

The following features and bug fixes have been added to the
applications since the 4.4.0 release. Additional detail for
each item listed below may be found on our community
website (www.xtuple.org).

New Features:

* Implement cash based VAT tax distribution [23253]
* Add the ability to enter an alternate exchange rate on a Cash Receipt 
[23254]
* Expose More Widgets Functions to Scripting [7417]
* Hiding the Commission rate from the customer entry screen [7622]

Bug Fixes:

* Possible to correct receivings on vouchered items [23511]
* Incomplete search via ellipses when attaching addresses and contacts 
in CRM, Vendors, etc [7202]
* Forward Update on Parent Updates Child Comp GL Accnts [7405]
* Error in Sales Return [7451]
* Reassign lot/serial creates duplicate lot numbers for lot controlled 
items [7497]
* On Item Record Creation Cannot Create Item Site: AVG Cost [7519]
* "View Item Costing" displays blank screen [7432]
* Distribute Stock Display of Lot/Location Data Wrong [7371]
* Error when inserting into api.glaccount [7411]
* Report: Work Order History prints empty [7408]
* No locations available in distribute stock FROM screen [7539]
* Characteristic value is not displayed in "Vendors" screen [23671]
* CM's do not credit cost of goods sold properly on multi quantity 
[23571]
* DB log error is generated on selecting to query the "Tax History" 
screen [23727]
* Distribute stock TO location screen does not display qty before [7538]
* Tax Figures off by 1 cent [23570]
* New margin column should be link to privilege [23468]
* Line items during transfer fails in error message [5810]
* Selecting to edit an item generates a DB log error [7322]
* Unclear How AVG Cost For MFG Item is Calaculated - No Variance [7479]
* TOs Do Not Transfer Average Cost [7520]
* Function Exec Sequence Post Operations - AVG Cost Item [7524]
* Can overload UOM input [6495]
* FRE Trend Income Statement Wrong Col Heading [6851]
* Figures in the amount field are not completely visible [7418]
* QOH not updating as expected on Transfers [7540]
* Transfer order shipments appear as not posted in inventory history 
[7439]
* Multi-Company - Cannot Use User Groups on Subsidiary [7403]
* Should Not Be Able to Uncheck Adjust Value When... [7530]
* Scrap Factor Displays as %1000 not %10 [7511]
* Unable to Connect Between DBs: Consolidate Companies [7226]
* Trend report on the Financial Report Writer mixes up columns [7156]
* Maintain External Shipping Records Crashes on Second Save [6967]
* Unable to Add Priv That Was Created Through Package Manager Import 
[7486]
* Incorrect display of Tax code on Invoice Item window [7470]
* Search Window for Accounts or Addresses, not sorting on column click 
[7176]
* tax for invoice items with a tax code of none but a non-0 tax is not 
recorded in the g/l [7522]
* Selecting to relate a CRM account as a Vendor, displays error [7422]
* New Incident data entry [7221]
* Rounding when vouchering [23580]
* Cannot Select Account From List Into Account Field [7478]
* Warehouse transfers for average costed items do not record cost 
movement [7436]
* Costs can get out of whack by doing average cost adjustments [7525]
* Selecting to post G/L series entries displays error [7427]
* Cannot create site without address [7414]
* GL account list is empty when no companies are used [7413]
* Updater 2.0.0Beta2 Error: You must supply a Shipto ID [7294]
* Function fetchnextnumber does not work for non-public tables [23100]
* Time In and Time Out columns are not populated [23757]
* Line item detail does not print on grade 0 report [7452]
* Report: PickingListNoClosedLines [7579]
* Upgrading 3.0.1 demo db gives cashrcpt error [7603]