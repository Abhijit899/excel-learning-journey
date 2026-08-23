Mini Project — SAP PO Priority Flagging System 250 rows
Scenario: Your manager at Mahindra wants every PO automatically flagged the moment the sheet opens — no manual review, using increasingly specific rules. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "PO Priority Flagging" (double-click tab)
2. In column J, use =IF(H2>150000,"High Value","Normal") for a simple amount-based flag
3. In column K, use =IF(I2="Delayed","Delayed Flag","On Track") for a simple status-based flag
4. In column L, use =IF(AND(H2>150000,I2="Delayed"),"🔴 Priority","🟢 Normal") combining both conditions
5. In column M, use =IF(AND(H2>150000,I2="Delayed",F2="North"),"🔴🔴 Critical North Priority","Normal") — a 3-condition AND test specific to North region
6. Apply Conditional Formatting: Text Contains "Priority" on column L → Red Fill
7. Apply Conditional Formatting: Text Contains "Critical" on column M → Dark Red Fill with bold text
8. Turn on AutoFilter and filter column L to show only "🔴 Priority" rows — note how many need urgent attention
9. Clear the filter, then add a Summary block starting P1: P1="Total Rows", Q1=250; P2="Priority POs (L)", Q2=count you observed; P3="Critical North POs (M)", Q3=count you observed
10. Save using Ctrl+S, then Save As (F12) → name it: new-day-06-if-ifand-mahindra-po.xlsx
11. Create Sheet2 → rename "IF Formula Log" → write down every formula used today with one line on what it does
12. Bold and underline the header row (Day 1)
13. Turn on AutoFilter, apply a Text Filter (Contains "Steel") on Vendor Name, then clear (Day 2)
14. Select PO Amount → Data Validation → Allow Custom → Formula ensuring value is greater than 0 (Day 3)
15. Use Flash Fill (Ctrl+E) if any text pattern extraction is useful on Vendor Name (Day 4)
16. Type 1.05 in a helper cell → copy → Paste Special Multiply on PO Amount for a 5% test revision, then undo (Day 5)



ANSWER : 


