Business Question Answer in 1 line
A SAP MM consultant's PO export has accidental duplicate rows (same PO ID entered twice by the system), AND every PO Amount needs a bulk 8% price revision applied at once.
Which specific feature removes duplicates permanently, and which specific Paste Special operation applies the bulk revision without writing 250 individual formulas?


ANSWER : 


Data → Remove Duplicates removes duplicate rows, and Paste Special → Multiply applies the 8% bulk revision.




---



Hard Question — Full Duplicate Removal & Paste Special Drill 230 rows (10 intentional duplicates) · single combined question
Paste this data. Notice 10 PO IDs appear twice on purpose. Complete every task below in order:

Duplicates & UNIQUE:
1. Select the full data range → Data → Remove Duplicates → tick "My data has headers" → tick only the PO ID column → OK — confirm Excel reports removing 10 duplicate rows
2. Undo (Ctrl+Z) to restore all 230 rows including duplicates
3. In a blank area (K1), use =UNIQUE(A2:A231) to list distinct PO IDs live, without deleting anything from the original data
4. In L1, use =COUNTA(UNIQUE(A2:A231)) to count exactly how many distinct PO IDs exist
5. Compare: L1 should show fewer than 230 — confirm the difference matches the 10 duplicates
6. Now actually run Remove Duplicates for real (Data → Remove Duplicates, PO ID column only) and keep the cleaned result this time
Paste Special:
7. Type 1.08 in any blank cell → copy it (Ctrl+C) → select PO Amount column → Ctrl+Alt+V → Multiply → OK — applies an 8% bulk price increase
8. Copy the Vendor Name column → paste it Transposed into a new area to see it flipped into a row
9. Add a formula column (e.g. GST = PO Amount × 0.18) → copy it → Ctrl+Alt+V → Values Only on top of itself, to freeze the results and remove the formula
10. Copy a short list containing a few blank cells → paste onto existing data using Ctrl+Alt+V → tick Skip Blanks → confirm existing data isn't overwritten
🔁 Revision (New Day 1-4):
11. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
12. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
13. Select Delivery Status column → Data Validation → Allow List → Delivered,Pending,Delayed (Day 3)
14. Select the full row range → New Rule → formula =$I2>200000 → Light Red Fill on the entire row (Day 4)


ANSWER : 


<img width="1383" height="5547" alt="Picture 36" src="https://github.com/user-attachments/assets/49ed0282-08cd-4fe4-a554-78d6390caaf5" />


<img width="1911" height="911" alt="Screenshot 2026-08-23 070724" src="https://github.com/user-attachments/assets/2a2ffbf8-5f17-444b-ad99-b52b744ca86f" />


<img width="1915" height="1020" alt="Screenshot 2026-08-23 070319" src="https://github.com/user-attachments/assets/d969a030-5a92-4289-a6dd-bebcf55f8fed" />


<img width="1898" height="912" alt="Screenshot 2026-08-23 071956" src="https://github.com/user-attachments/assets/d83774f2-9a50-4403-ba1b-dea92bd5e7e1" />



<img width="1505" height="5565" alt="Picture 37" src="https://github.com/user-attachments/assets/caa3426c-4739-4a71-94dd-e834c802d392" />


<img width="1702" height="5565" alt="Picture 38" src="https://github.com/user-attachments/assets/110f5bc8-da86-453a-8813-2ea65d38e5c2" />


<img width="1702" height="5565" alt="Picture 40" src="https://github.com/user-attachments/assets/950e1388-a20c-4941-8fd6-e67099b691f4" />


<img width="1743" height="5565" alt="Picture 41" src="https://github.com/user-attachments/assets/36e8bcfd-81b6-46fe-9c30-6e75df5e1579" />

