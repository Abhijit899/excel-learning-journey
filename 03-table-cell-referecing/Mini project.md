Mini Project — SAP Smart PO Register with Tables & References 120 rows
Scenario: You are a junior SAP MM consultant at L&T. Your manager wants a smart, dynamic PO register that automatically calculates taxes, shows budget variance, and has a clean summary sheet — all linked using proper cell referencing.

Sheet 1 — "PO Register":
1. Paste 120-row data → Convert to Table → name it "LTPOTable"
2. Apply professional table style (Medium Style 9 — dark blue)
3. Enable Total Row

Rate Setup area (cols M–N in Sheet 1):
M1=GST Rate | N1=18%
M2=Budget per PO | N2=400000
M3=Discount | N3=2%

Add calculated columns in table:
Col K — GST Amount: =[@[PO Amount]]*$N$1
Col L — Total with GST: =[@[PO Amount]]+[@[GST Amount]]
Col M — Budget Variance: =[@[PO Amount]]-$N$2 (positive = over budget, negative = under)
Col N — Discount Amount: =[@[Total with GST]]*$N$3
Col O — Final Payable: =[@[Total with GST]]-[@[Discount Amount]]
Col P — Rounded Final: =ROUND([@[Final Payable]],0)

Conditional Formatting (revision):
— Delivery Status = Delayed → Orange row
— Delivery Status = Pending → Yellow row
— Budget Variance positive (above budget) → Red font
— Final Payable above 500000 → Bold Red

Sorting (revision):
— Sort by Payment Status custom order: Overdue → Pending → Paid
— Then by Final Payable largest to smallest

Sheet 2 — "Summary Dashboard":
All values using cross-sheet references and structured references only:
— Total PO Amount: =SUM(LTPOTable[PO Amount])
— Total GST: =SUM(LTPOTable[GST Amount])
— Total Final Payable: =SUM(LTPOTable[Final Payable])
— Average PO: =AVERAGE(LTPOTable[PO Amount])
— Highest PO: =MAX(LTPOTable[PO Amount])
— Lowest PO: =MIN(LTPOTable[PO Amount])
— Total Entries: =COUNTA(LTPOTable[PO ID])
— GST Rate used: ='PO Register'!N1
— Budget per PO: ='PO Register'!N2


ANSWER : 




Sheet 1 — "PO Register":
1. Paste 120-row data → Convert to Table → name it "LTPOTable"
2. Apply professional table style (Medium Style 9 — dark blue)
3. Enable Total Row

Rate Setup area (cols M–N in Sheet 1):
M1=GST Rate | N1=18%
M2=Budget per PO | N2=400000
M3=Discount | N3=2%

Add calculated columns in table:
Col K — GST Amount: =[@[PO Amount]]*$N$1
Col L — Total with GST: =[@[PO Amount]]+[@[GST Amount]]
Col M — Budget Variance: =[@[PO Amount]]-$N$2 (positive = over budget, negative = under)
Col N — Discount Amount: =[@[Total with GST]]*$N$3
Col O — Final Payable: =[@[Total with GST]]-[@[Discount Amount]]
Col P — Rounded Final: =ROUND([@[Final Payable]],0)



ANSWERS : 


<img width="2551" height="2909" alt="Picture1" src="https://github.com/user-attachments/assets/b7841737-6107-476a-8471-309840a4a6ed" />


Conditional Formatting (revision):
— Delivery Status = Delayed → Orange row
— Delivery Status = Pending → Yellow row
— Budget Variance positive (above budget) → Red font
— Final Payable above 500000 → Bold Red

Sorting (revision):
— Sort by Payment Status custom order: Overdue → Pending → Paid
— Then by Final Payable largest to smallest

ANSWER :


<img width="3763" height="2909" alt="Picture 2" src="https://github.com/user-attachments/assets/129018b5-e43c-4c5e-9304-955b07cc9a18" />



Sheet 2 — "Summary Dashboard":
All values using cross-sheet references and structured references only:
— Total PO Amount: =SUM(LTPOTable[PO Amount])
— Total GST: =SUM(LTPOTable[GST Amount])
— Total Final Payable: =SUM(LTPOTable[Final Payable])
— Average PO: =AVERAGE(LTPOTable[PO Amount])
— Highest PO: =MAX(LTPOTable[PO Amount])
— Lowest PO: =MIN(LTPOTable[PO Amount])
— Total Entries: =COUNTA(LTPOTable[PO ID])
— GST Rate used: ='PO Register'!N1
— Budget per PO: ='PO Register'!N2




