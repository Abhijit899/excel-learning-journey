Mini Project — SAP Duplicate-Free PO Master with Bulk Price Update 250 rows (12 intentional duplicates)
Scenario: Your manager at Mahindra just found out the SAP export tool has a bug that occasionally double-enters POs, and separately wants a 10% price revision applied company-wide before quarter close. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "PO Master Cleanup" (double-click tab)
2. In a helper area, use =UNIQUE(A2:A251) to preview the distinct PO ID list before deleting anything
3. Use =COUNTA(UNIQUE(A2:A251)) to confirm exactly how many duplicates exist (should be 12)
4. Run Data → Remove Duplicates on the PO ID column → confirm the report matches your UNIQUE count
5. Type 1.10 in a helper cell → copy it → select PO Amount column → Ctrl+Alt+V → Multiply → OK — applies the 10% price revision
6. Add a formula column for GST (PO Amount × 0.18) → copy → Paste Special → Values Only on itself to lock in the numbers
7. Copy the cleaned Vendor Name column → Paste Special → Transpose into a new area for a quick horizontal reference list
8. Apply Currency formatting (Ctrl+Shift+$) on the updated PO Amount column
9. Add a Summary block starting L1: L1="Duplicates Removed", M1=count you observed; L2="Price Revision Applied", M2="+10% via Paste Special Multiply"; L3="Final Row Count", M3=value after cleanup
10. Save using Ctrl+S, then Save As (F12) → name it: new-day-05-duplicates-pastespecial-mahindra-po.xlsx
11. Create Sheet2 → rename "Cleanup & Paste Special Log" → write down every step and formula used today
12. Bold and underline the header row (Day 1)
13. Turn on AutoFilter, filter Delivery Status = "Delayed", then clear (Day 2)
14. Use Text to Columns or Flash Fill if any combined text columns are present (Day 4)
15. Apply a 3-Color Scale on the updated PO Amount column (Day 4)




ANSWER : 



<img width="2102" height="5758" alt="Picture 42" src="https://github.com/user-attachments/assets/890a2a65-b985-4cbe-8549-5ca02e15cd52" />


<img width="2102" height="1736" alt="Picture 43" src="https://github.com/user-attachments/assets/90d38909-5972-4215-9622-bbc22a108c1d" />


<img width="2102" height="1736" alt="Picture 44" src="https://github.com/user-attachments/assets/eac3c07c-a019-499f-8b06-d7e3f9ab3e7a" />

