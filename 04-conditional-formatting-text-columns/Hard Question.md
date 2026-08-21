Business Question Answer in 1 line

A SAP MM consultant has a single column containing "Vendor Name - Vendor ID" combined (e.g. "Tata Steel - V-001") and needs it split into two clean columns without writing any formula. 
Separately, they want the ENTIRE row highlighted red wherever PO Amount exceeds ₹200000. Which specific feature solves each of these two problems?


ANSWER : 

Text to Columns + Conditional Formatting.


---



Hard Question — Full Conditional Formatting & Text Splitting Drill 220 rows · single combined question
Paste this data. Notice column C is "Vendor Name - Vendor ID" combined into ONE cell, on purpose. Complete every task below in order:

Text to Columns & Flash Fill:
1. Select column C → Data → Text to Columns → Delimited → tick "Other" and type a dash (-) as the delimiter → set Destination to a new empty area (e.g. K1) → Finish — confirm Vendor Name and Vendor ID now sit in 2 separate columns
2. Undo that (Ctrl+Z) to restore the combined column
3. In L2, manually type just "Tata Steel" (the Vendor Name part only, copied from C2) → select L2:L221 → press Ctrl+E (Flash Fill) → confirm it extracts every Vendor Name automatically, without Text to Columns
4. In M2, manually type just "V-001" (the Vendor ID part only) → select M2:M221 → press Ctrl+E → confirm it extracts every Vendor ID
Conditional Formatting:
5. Select PO Amount column (H2:H221) → Highlight Cells Rules → Greater Than → 200000 → Light Red Fill
6. Select Qty column → Top/Bottom Rules → Top 10 Items → Green Fill
7. Apply a 3-Color Scale on PO Amount
8. Apply Data Bars (Blue Gradient) on Qty
9. Select A2:I221 → New Rule → Use a formula → =$H2>200000 → Light Red Fill → confirms the entire row highlights, not just column H
10. Select the Vendor ID column (M2:M221 from your Flash Fill result) → Highlight Cells Rules → Duplicate Values → Light Yellow Fill
11. Open Manage Rules → tick "Stop If True" on the row-highlight formula rule so it takes priority
12. Use the Name Box to jump directly to L1, then Ctrl+Home back to A1 (Day 1)
13. Use =SUM(H2:H221) with Alt+= to confirm total PO value (Day 1)
14. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
15. Turn on AutoFilter (Ctrl+Shift+L), filter Delivery Status = "Delayed", then clear (Day 2)
16. Select Qty column → Data Validation → Allow Whole Number → Between 1 and 100 (Day 3)




ANSWER : 







