Mini Project — SAP Vendor Data Cleaning + PO Report 120 rows
Scenario: You are a junior SAP MM consultant at Bajaj Auto. The SAP team exports vendor and PO data but it comes in messy format — ALL CAPS names, combined city+state, extra spaces, amounts as text, dates in wrong format. Your manager needs a clean professional report in 2 hours.

Sheet 1 — "Raw Data": paste 120-row dataset

Step 1 — Text cleaning columns:
Col L — Clean Vendor Name: =PROPER(TRIM(D2))
Col M — City: =LEFT(F2,FIND(",",F2)-1)
Col N — State: =TRIM(MID(F2,FIND(",",F2)+1,LEN(F2)))
Col O — PO Number only: =RIGHT(A2,4)
Col P — Category Proper: =PROPER(H2)
Col Q — PO Label: =A2&" | "&PROPER(TRIM(D2))&" | "&E2

Step 2 — Math columns (revision Day 4):
Col R — GST 18%: =ROUND(I2*18%,2)
Col S — Total with GST: =I2+R2
Col T — Rounded Total: =ROUNDUP(S2,0)
Col U — Budget Variance: =ABS(I2-400000)

Step 3 — Conditional Formatting (revision):
— Delivery=Delayed → Orange row
— Delivery=Pending → Yellow row
— Delivery=Delivered → Green row
— Total with GST above 600000 → Red fill

Step 4 — Sorting (revision):
— Payment Status custom: Overdue → Pending → Paid
— Then Total with GST largest to smallest


Sheet 2 — "Summary":
— Total PO Amount: SUM
— Total GST: SUM
— Total with GST: SUM
— Average PO: AVERAGE
— Highest PO: MAX | 2nd Highest: LARGE(,2)
— Lowest PO: MIN
— Total Entries: COUNTA
— Count Delayed: COUNTIF
— Count Overdue: COUNTIF


ANSWERS : 



Sheet 1 — "Raw Data": paste 120-row dataset

Step 1 — Text cleaning columns:
Col L — Clean Vendor Name: =PROPER(TRIM(D2))
Col M — City: =LEFT(F2,FIND(",",F2)-1)
Col N — State: =TRIM(MID(F2,FIND(",",F2)+1,LEN(F2)))
Col O — PO Number only: =RIGHT(A2,4)
Col P — Category Proper: =PROPER(H2)
Col Q — PO Label: =A2&" | "&PROPER(TRIM(D2))&" | "&E2


ANS .


<img width="3280" height="2879" alt="Picture 37" src="https://github.com/user-attachments/assets/fe58999a-9a16-4e48-bca3-af05055de514" />


Step 2 — Math columns (revision Day 4):
Col R — GST 18%: =ROUND(I2*18%,2)
Col S — Total with GST: =I2+R2
Col T — Rounded Total: =ROUNDUP(S2,0)
Col U — Budget Variance: =ABS(I2-400000)


ANS . 


<img width="4562" height="2879" alt="Picture 38" src="https://github.com/user-attachments/assets/71fd4a92-7cd6-4e2a-8117-762637b7b521" />


Step 3 — Conditional Formatting (revision):
— Delivery=Delayed → Orange row
— Delivery=Pending → Yellow row
— Delivery=Delivered → Green row
— Total with GST above 600000 → Red fill


ANS . 


<img width="4562" height="2879" alt="Picture 39" src="https://github.com/user-attachments/assets/8c5aa870-48e7-4b3f-be4e-90056e6f937d" />



Step 4 — Sorting (revision):
— Payment Status custom: Overdue → Pending → Paid
— Then Total with GST largest to smallest


ANS . 


<img width="4562" height="2879" alt="Picture 40" src="https://github.com/user-attachments/assets/dfdbc7b5-1a71-4b27-8ae7-476d05bcadcd" />





Sheet 2 — "Summary":
— Total PO Amount: SUM
— Total GST: SUM
— Total with GST: SUM
— Average PO: AVERAGE
— Highest PO: MAX | 2nd Highest: LARGE(,2)
— Lowest PO: MIN
— Total Entries: COUNTA
— Count Delayed: COUNTIF
— Count Overdue: COUNTIF


ANS . 


<img width="516" height="447" alt="Screenshot 2026-07-22 111906" src="https://github.com/user-attachments/assets/9e0469aa-1c5c-4719-abe9-63c614d73991" />

