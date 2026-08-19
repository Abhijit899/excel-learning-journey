Mini Project — SAP Clean Intake Sheet with Vendor Extraction 250 rows
Scenario: Your manager at Mahindra wants a fresh intake sheet where data entry mistakes are impossible going forward, PLUS a quick extracted list of every high-priority PO (North region OR high value) for tomorrow's review. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "Clean Intake Setup" (double-click tab)
2. Set up a Criteria Range for: Region="North" OR PO Amount>200000 (2 separate rows, matching column headers copied above)
3. Run Advanced Filter with that criteria, Copy to a new area starting at L1
4. Separately, extract a Unique list of all Category values into a new area using "Unique records only"
5. Apply Data Validation on Delivery Status column: Allow List → Delivered,Pending,Delayed
6. Apply Data Validation on Region column: Allow List → North,South,East,West
7. Apply Data Validation on Qty column: Allow Whole Number → Between 1 and 100, with an Input Message explaining the rule
8. Apply Data Validation on PO Amount column: Allow Custom → Formula ensuring value is greater than 0, with a clear Error Alert message
9. Use Circle Invalid Data to check the whole sheet for any rule violations already present
10. Add a Summary block starting from cell P1: P1="High-Priority POs Extracted", Q1=count you observed; P2="Unique Categories Found", Q2=count you observed; P3="Validation Rules Applied", Q3=4
11. Save using Ctrl+S, then Save As (F12) → name it: new-day-03-advfilter-datavalidation-mahindra-po.xlsx
12. Create Sheet2 → rename "Filter & Validation Log" → write down every criteria range and validation rule used today
13. Select PO Amount → Ctrl+Shift+$ Currency format (Day 1)
14. Bold and underline the header row using Ctrl+B then Ctrl+U (Day 1)
15. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
16. Turn on AutoFilter, apply a Text Filter (Contains "Steel") on Vendor Name, then clear it (Day 2)


ANSWER :


