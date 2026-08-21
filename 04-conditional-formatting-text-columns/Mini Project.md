Mini Project — SAP Vendor Column Cleanup & Risk Dashboard 250 rows
Scenario: Your manager at Mahindra receives this export monthly with the Vendor column always combined, and always wants problem POs flagged visually before the review call. Build a repeatable setup. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "Vendor Cleanup & Risk" (double-click tab)
2. Use Text to Columns on column C (Delimited, dash separator) → split into Vendor Name and Vendor ID in a fresh destination area
3. In a separate helper column, use Flash Fill (Ctrl+E) to achieve the same Vendor Name split, typing one example first
4. Apply a 3-Color Scale on PO Amount
5. Apply Data Bars on Qty
6. Select the full row range → New Rule → formula =$H2>200000 → Light Red Fill for high-value row highlighting
7. Select the full row range → New Rule → formula =$I2="Delayed" → Light Yellow Fill for delayed row highlighting
8. Open Manage Rules → set "Stop If True" on the high-value rule so it takes priority over the delayed rule
9. Apply Highlight Cells Rules → Duplicate Values on your split Vendor ID column
10. Add a Summary block starting L1: L1="High-Value POs (>200000)", M1=count you observed; L2="Delayed POs", M2=count you observed; L3="Duplicate Vendor Rows", M3=count you observed
11. Save using Ctrl+S, then Save As (F12) → name it: new-day-04-condformat-texttocolumns-mahindra-po.xlsx
12. Create Sheet2 → rename "CF & Text Split Log" → write down every rule and split method used today
13. Select PO Amount → Ctrl+Shift+$ Currency format (Day 1)
14. Bold and underline the header row (Day 1)
15. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
16. Select Delivery Status column → Data Validation → Allow List → Delivered,Pending,Delayed (Day 3)



ANSWER : 


<img width="1410" height="6027" alt="Picture 33" src="https://github.com/user-attachments/assets/1f8615f0-56c1-4167-ab90-3dcc91eb86eb" />


<img width="1410" height="6027" alt="Picture 34" src="https://github.com/user-attachments/assets/4230a6ce-9edd-4be2-8176-76aee21c3cea" />


<img width="1410" height="6027" alt="Picture 35" src="https://github.com/user-attachments/assets/9dc9a834-32da-44fe-8bc5-389b07cb2bee" />


<img width="1802" height="998" alt="Screenshot 2026-08-21 210740" src="https://github.com/user-attachments/assets/22eed810-8063-42e5-91f4-5a42151cbd5a" />
