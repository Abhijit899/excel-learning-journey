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


---


Hard Q2 — SAP Invoice Register — Mixed References 80 rows
This dataset has multiple tax rates. Use cell referencing correctly for each:

Setup first:
In a rate table area (cols K–L) type this:
K1=Category | L1=Tax Rate
K2=Raw Material | L2=5%
K3=Machinery | L3=12%
K4=Chemicals | L4=18%
K5=IT Equipment | L5=18%
K6=Packaging | L6=12%
K7=Office Supplies | L7=5%
K8=Logistics | L8=18%
K9=Utilities | L9=5%

Tasks:
1. Convert data to table — name it "InvoiceTable"
2. Add column "CGST 9%" = [@[Invoice Amount]]*9% using structured reference
3. Add column "SGST 9%" = [@[Invoice Amount]]*9%
4. Add column "Total GST" = [@CGST]+[@SGST]
5. Add column "Total Payable" = [@[Invoice Amount]]+[@[Total GST]]
6. In cell A85 type "Fixed Discount" and B85 = 5000
7. Add column "After Discount" = [@[Total Payable]]-$B$85 → drag down → confirm B85 stays fixed
8. Add column "Rounded Total" = ROUND([@[After Discount]],0)
9. In Sheet 2 "Invoice Summary" add:
   Total Invoice Amount: =SUM(InvoiceTable[Invoice Amount])
   Total GST: =SUM(InvoiceTable[Total GST])
   Total Payable: =SUM(InvoiceTable[Total Payable])
   Average Invoice: =AVERAGE(InvoiceTable[Invoice Amount])
10. Apply CF on Total Payable column: above 500000 = Red fill, below 200000 = Green fill (revision)
11. Sort InvoiceTable by Total Payable largest to smallest (revision)
12. Filter InvoiceTable — State = Maharashtra (revision)


ANSWERS : 


1. Convert data to table — name it "InvoiceTable"
2. Add column "CGST 9%" = [@[Invoice Amount]]*9% using structured reference
3. Add column "SGST 9%" = [@[Invoice Amount]]*9%
4. Add column "Total GST" = [@CGST]+[@SGST]
5. Add column "Total Payable" = [@[Invoice Amount]]+[@[Total GST]]
6. In cell A85 type "Fixed Discount" and B85 = 5000
7. Add column "After Discount" = [@[Total Payable]]-$B$85 → drag down → confirm B85 stays fixed
8. Add column "Rounded Total" = ROUND([@[After Discount]],0)
9. In Sheet 2 "Invoice Summary" add:
   Total Invoice Amount: =SUM(InvoiceTable[Invoice Amount])
   Total GST: =SUM(InvoiceTable[Total GST])
   Total Payable: =SUM(InvoiceTable[Total Payable])
   Average Invoice: =AVERAGE(InvoiceTable[Invoice Amount])
10. Apply CF on Total Payable column: above 500000 = Red fill, below 200000 = Green fill (revision)

Ans. 

<img width="2258" height="1945" alt="Picture 16" src="https://github.com/user-attachments/assets/b2774dc9-3391-4c70-bfbc-d5e5f9da68a7" />


11. Sort InvoiceTable by Total Payable largest to smallest (revision)

Ans . 

<img width="2258" height="1945" alt="Picture 17" src="https://github.com/user-attachments/assets/59e1dd25-32f7-4f81-9509-b0a4d1ceb045" />


12. Filter InvoiceTable — State = Maharashtra (revision)

Ans. 

<img width="2258" height="193" alt="Picture 18" src="https://github.com/user-attachments/assets/1b46a0cd-498d-4640-a21d-00a6566ddf11" />
