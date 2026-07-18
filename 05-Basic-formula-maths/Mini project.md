Mini Project — SAP Monthly PO Financial Summary 120 rows
Scenario: You are a junior SAP MM consultant at Tata Motors. Every month end you prepare a financial summary of all Purchase Orders — calculating GST, rounding for compliance, finding top/bottom vendors, and building a summary dashboard.

Sheet 1 — "PO Register": paste 120-row data

Rate Setup (outside table in cols N–O):
N1=GST Rate | O1=18%
N2=Budget | O2=400000
N3=Instalment Count | O3=3

Add columns inside table:
Col L — GST Amount: =ROUND([@[PO Amount]]*$O$1,2)
Col M — GST RoundUp: =ROUNDUP([@[PO Amount]]*$O$1,0)
Col N — Total with GST: =[@[PO Amount]]+[@[GST Amount]]
Col O — Total RoundUp: =ROUNDUP([@[Total with GST]],0)
Col P — Total to nearest 1000: =MROUND([@[Total with GST]],1000)
Col Q — Budget Variance: =ABS([@[PO Amount]]-$O$2)
Col R — Instalment: =ROUNDDOWN([@[Total with GST]]/$O$3,0)
Col S — Floor to nearest 500: =FLOOR([@[PO Amount]],500)
Col T — Ceiling to nearest 500: =CEILING([@[PO Amount]],500)

Conditional Formatting (revision):
— Delivery=Delayed → Orange row | Pending → Yellow | Delivered → Green
— Budget Variance above 200000 → Bold Red font
— Total with GST above 600000 → Red fill

Sorting (revision):
— Payment Status custom: Overdue → Pending → Paid
— Then Total with GST largest to smallest

Sheet 2 — "Financial Summary":
Overall:
— Total PO Amount: SUM
— Total GST: SUM
— Total with GST: SUM
— Average PO: AVERAGE
— Highest PO: MAX | 2nd Highest: LARGE(,2) | 3rd Highest: LARGE(,3)
— Lowest PO: MIN | 2nd Lowest: SMALL(,2)
— Total Entries: COUNTA




ANSWERS : 



Sheet 1 — "PO Register": paste 120-row data

Rate Setup (outside table in cols N–O):
N1=GST Rate | O1=18%
N2=Budget | O2=400000
N3=Instalment Count | O3=3

ANS . 


<img width="1550" height="2850" alt="Picture 24" src="https://github.com/user-attachments/assets/d7c1084a-65b0-4f0c-831b-f9f7367b34c9" />


Add columns inside table:
Col L — GST Amount: =ROUND([@[PO Amount]]*$O$1,2)
Col M — GST RoundUp: =ROUNDUP([@[PO Amount]]*$O$1,0)
Col N — Total with GST: =[@[PO Amount]]+[@[GST Amount]]
Col O — Total RoundUp: =ROUNDUP([@[Total with GST]],0)
Col P — Total to nearest 1000: =MROUND([@[Total with GST]],1000)
Col Q — Budget Variance: =ABS([@[PO Amount]]-$O$2)
Col R — Instalment: =ROUNDDOWN([@[Total with GST]]/$O$3,0)
Col S — Floor to nearest 500: =FLOOR([@[PO Amount]],500)
Col T — Ceiling to nearest 500: =CEILING([@[PO Amount]],500)

ANS . 


<img width="4136" height="2850" alt="Picture 25" src="https://github.com/user-attachments/assets/d2af7919-1229-44df-82a6-9cd20ecf3e5b" />



Conditional Formatting (revision):
— Delivery=Delayed → Orange row | Pending → Yellow | Delivered → Green
— Budget Variance above 200000 → Bold Red font
— Total with GST above 600000 → Red fill

ANS .


<img width="4136" height="2850" alt="Picture 26" src="https://github.com/user-attachments/assets/952e2037-97e3-4c0a-9061-00d72b6777d3" />

Sorting (revision):
— Payment Status custom: Overdue → Pending → Paid
— Then Total with GST largest to smallest

ANS . 


<img width="4136" height="2850" alt="Picture 27" src="https://github.com/user-attachments/assets/9a0b85b8-c679-49a2-897d-8110f0063e62" />


Sheet 2 — "Financial Summary":
Overall:
— Total PO Amount: SUM
— Total GST: SUM
— Total with GST: SUM
— Average PO: AVERAGE
— Highest PO: MAX | 2nd Highest: LARGE(,2) | 3rd Highest: LARGE(,3)
— Lowest PO: MIN | 2nd Lowest: SMALL(,2)
— Total Entries: COUNTA

ANS .


<img width="619" height="437" alt="Screenshot 2026-07-18 150229" src="https://github.com/user-attachments/assets/c1a34e53-3eb1-43ec-86ac-1869494d2bbe" />


