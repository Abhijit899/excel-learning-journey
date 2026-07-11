Hard Q1 — SAP PO Table Creation + Referencing 80 rows
Paste this data in Excel and complete all tasks:

Table Creation Tasks:
1. Select entire data range → Ctrl+T → tick "My table has headers" → OK
2. Rename table to "POTable" in Table Design tab
3. Apply Table Style — Medium Style 2 (blue theme)
4. Enable Total Row → set PO Amount column to SUM → Qty column to SUM → what are the totals?
5. Add a new column in the table "GST Amount" — type formula in first cell only → it fills entire column automatically:
   =[@[PO Amount]]*18% (structured reference — table fills automatically)
6. Add another column "Total with GST" = [@[PO Amount]]+[@[GST Amount]]
7. Filter table: Delivery Status = Delayed — how many rows?
8. Sort table: PO Amount largest to smallest directly from table header dropdown
9. Add a new row at bottom — PO-MM-1081, 15-07-2026, Sun Pharma, V-020, West, Maharashtra, Chemicals, 25, 345000, Pending, Paid — confirm table expands automatically

Cell Referencing Tasks:
10. In cell N1 type "GST Rate" and in N2 type 18%
11. In column O add "GST using Absolute" = H2*$N$2 → drag down all 80 rows → compare with column M (structured ref) — both should match
12. In column P add "Budget Variance" — Budget is fixed at 300000 in cell P1:
   =H2-$P$1 → drag down — shows how much each PO is above or below budget


   ANSWERS :


Table Creation Tasks:
1. Select entire data range → Ctrl+T → tick "My table has headers" → OK
2. Rename table to "POTable" in Table Design tab
3. Apply Table Style — Medium Style 2 (blue theme)
4. Enable Total Row → set PO Amount column to SUM → Qty column to SUM → what are the totals?
5. Add a new column in the table "GST Amount" — type formula in first cell only → it fills entire column automatically:
   =[@[PO Amount]]*18% (structured reference — table fills automatically)
6. Add another column "Total with GST" = [@[PO Amount]]+[@[GST Amount]]
7. Filter table: Delivery Status = Delayed — how many rows?
8. Sort table: PO Amount largest to smallest directly from table header dropdown
9. Add a new row at bottom — PO-MM-1081, 15-07-2026, Sun Pharma, V-020, West, Maharashtra, Chemicals, 25, 345000, Pending, Paid — confirm table expands automatically


Ans .

1. Select entire data range → Ctrl+T → tick "My table has headers" → OK
2. Rename table to "POTable" in Table Design tab
3. Apply Table Style — Medium Style 2 (blue theme)
4. Enable Total Row → set PO Amount column to SUM → Qty column to SUM → what are the totals?
5. Add a new column in the table "GST Amount" — type formula in first cell only → it fills entire column automatically:
   =[@[PO Amount]]*18% (structured reference — table fills automatically)
6. Add another column "Total with GST" = [@[PO Amount]]+[@[GST Amount]]

Ans. 


<img width="1644" height="1969" alt="Picture 11" src="https://github.com/user-attachments/assets/dde4831c-67c8-464b-a64b-ca50407228e1" />


7. Filter table: Delivery Status = Delayed — how many rows?

Ans .

<img width="1644" height="625" alt="Picture 12" src="https://github.com/user-attachments/assets/100161f4-5043-4805-ac2f-82acb36c8e02" />


8. Sort table: PO Amount largest to smallest directly from table header dropdown

Ans.

<img width="1644" height="1969" alt="Picture 13" src="https://github.com/user-attachments/assets/c5bfa6da-7190-421f-ae9c-879d661c6bba" />


9. Add a new row at bottom — PO-MM-1081, 15-07-2026, Sun Pharma, V-020, West, Maharashtra, Chemicals, 25, 345000, Pending, Paid — confirm table expands automatically

Ans.


<img width="1644" height="1993" alt="Picture 14" src="https://github.com/user-attachments/assets/c25b4412-864a-467c-be03-a428b34ca89b" />



Cell Referencing Tasks:
10. In cell N1 type "GST Rate" and in N2 type 18%
11. In column O add "GST using Absolute" = H2*$N$2 → drag down all 80 rows → compare with column M (structured ref) — both should match
12. In column P add "Budget Variance" — Budget is fixed at 300000 in cell P1:
   =H2-$P$1 → drag down — shows how much each PO is above or below budget

ANSWERS:

<img width="1873" height="1993" alt="Picture 15" src="https://github.com/user-attachments/assets/7750e90c-2426-42ca-9742-1162f3a4667b" />

