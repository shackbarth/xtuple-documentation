Release Notes
xTuple ERP
Version 3.8.1
April 2, 2012
----------------------------------

These are the release notes for the 3.8.1 Patch Release. Thanks
to all who contributed to make this release possible.

As always, please review the xTuple Compatibility Matrix before
upgrading: http://www.xtuple.org/compatibility-matrix.

----------------------------------

The following features and bug fixes have been added to the
applications since the 3.8.1 release. Additional detail for
each item listed below may be found on our community
website (www.xtuple.org).

New Features:

N/A

Bug Fixes:

* [Observation]: S/O for a partially posted W/O deletes without a warning message [7683]
* applying two credit memos to cash receipt via multiselect does not work [16255]
* Enhanced Commissions tab disabled when entering a new Sales Rep [16490]
* Maintain shipping shows orders with 0 qty. at shipping [16589]
* Db error running as-of QOH config [16640]
* System does not allow PO return for an item with Control Method None [16757]
* Receiving against a drop-ship PO for an average cost item fails in the issue to
  shipping process with negative quantity message [16760]
* invhist insert problem [16764]
* calcsalesorderamt().sql function not filtering out cancelled line items [16781]
* Lead Time Analysis: User can edit itemsite without privilege to do so [16783]
* Voucher Distribution of Control Method None Items: Reject not correct [16829]
* Cannot delete G/L Series if using Journals [16834]
* deleteGLSeries reporting the wrong error message [16835]
* Voided invoices not found on customer history [16851]
* Voided tax authority check appears on bank rec [16861]
* Open Receivables gives wrong valuation [16873]
* Running MRP with exceptions nets a shortage [16890]
* When deleting an unposted invoice to which a credit memo has been applied,
  the system does not remove the allocation [16909]
* If a user does not have the ChgARInvcDistDate privilege, invoices are posted with
  the current date not the invoice date [16910]
* Edit sales history priv. required to edit AP Voucher [16928]
* One-sided transaction possible [16951]
* MRP fails when multiple revisions exist [16987]
