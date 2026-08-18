Mini Project — SAP Regional PO Ranking Report 250 rows
Scenario: Your manager at Mahindra wants a report ranked region-by-region with the biggest POs on top, and wants to quickly filter down to just the Delayed rows during the review call. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "Regional PO Ranking" (double-click tab)
2. Data → Sort → Level 1: Region (A to Z), Level 2: PO Amount (Largest to Smallest)
3. Turn on AutoFilter (Ctrl+Shift+L)
4. Filter Delivery Status to show only "Delayed"
5. Note how many rows remain, then clear the filter
6. Apply a Number Filter on PO Amount → Top 10 Items → note the top vendors
7. Clear filters, re-sort by PO ID (A to Z) to restore original order
8. Add a Summary block starting L1: L1="Sort Levels Used", M1=2; L2="Delayed Rows Found", M2=count you observed; L3="Top Vendor", M3=vendor you observed most
9. Save using Ctrl+S, then Save As (F12) → name it: new-day-02-sorting-filtering-mahindra-po.xlsx
10. Create Sheet2 → rename "Sort & Filter Log" → write down every sort level and filter condition used today
🔁 Revision (New Day 1, applied on this same report):
11. Use the Name Box to jump directly to L1, then Ctrl+Home back to A1
12. In a helper cell, use =SUM(I2:I251) with Alt+= to confirm total PO value on this report
13. In a helper cell, use =AVERAGE(I2:I251) to confirm the average PO Amount
14. Select PO Amount → Ctrl+Shift+$ Currency format
15. Bold and underline the header row using Ctrl+B then Ctrl+U


ANSWER : 


<img width="1138" height="6027" alt="Picture 13" src="https://github.com/user-attachments/assets/54bea857-ba4b-494c-a0f7-1b25198ea63b" />


<img width="1138" height="1827" alt="Picture 14" src="https://github.com/user-attachments/assets/44a47e79-6b94-4a61-b607-5f1b617b3ce9" />


<img width="1138" height="6075" alt="Picture 15" src="https://github.com/user-attachments/assets/11188b79-1d6a-41a4-99cc-09b71c348d3b" />


<img width="1571" height="427" alt="Screenshot 2026-08-18 213230" src="https://github.com/user-attachments/assets/62bc4598-4105-4dbe-bf47-6a4810e4902b" />
