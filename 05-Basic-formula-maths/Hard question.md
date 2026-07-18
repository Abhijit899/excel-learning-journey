Hard Q1 — SAP PO Amount Analysis 80 rows
Paste this SAP Purchase Order data and complete all formula tasks in a Summary area below the data (row 85 onwards):

Basic Formula Tasks:
1. Total PO Amount: =SUM(I2:I81)
2. Average PO Amount: =AVERAGE(I2:I81)
3. Highest PO Amount: =MAX(I2:I81)
4. Lowest PO Amount: =MIN(I2:I81)
5. Count of PO entries (numbers): =COUNT(I2:I81)
6. Count of PO IDs (text): =COUNTA(A2:A81)
7. 2nd Highest PO Amount: =LARGE(I2:I81,2)
8. 3rd Highest PO Amount: =LARGE(I2:I81,3)
9. 2nd Lowest PO Amount: =SMALL(I2:I81,2)
10. 3rd Lowest PO Amount: =SMALL(I2:I81,3)

Add calculated columns:
Col J — GST 18% Rounded to 2 decimals: =ROUND(I2*18%,2)
Col K — GST Rounded UP to nearest rupee: =ROUNDUP(I2*18%,0)
Col L — GST Rounded DOWN: =ROUNDDOWN(I2*18%,0)
Col M — Total with GST (using rounded): =I2+J2
Col N — Instalment 1 of 3 (round down): =ROUNDDOWN(I2/3,0)
Col O — Budget Variance ABS (budget=300000): =ABS(I2-300000)
Col P — PO Amount to nearest 1000 (FLOOR): =FLOOR(I2,1000)
Col Q — PO Amount rounded up to nearest 1000 (CEILING): =CEILING(I2,1000)
Col R — PO Amount to nearest 500 (MROUND): =MROUND(I2,500)

Revision tasks:
— Apply CF: PO Amount above 400000 = Red fill (revision)
— Sort by PO Amount Largest to Smallest (revision)
— Convert to table named "POAnalysis" (revision)


ANSWERS :


Basic Formula Tasks:
1. Total PO Amount: =SUM(I2:I81)
2. Average PO Amount: =AVERAGE(I2:I81)
3. Highest PO Amount: =MAX(I2:I81)
4. Lowest PO Amount: =MIN(I2:I81)
5. Count of PO entries (numbers): =COUNT(I2:I81)
6. Count of PO IDs (text): =COUNTA(A2:A81)
7. 2nd Highest PO Amount: =LARGE(I2:I81,2)
8. 3rd Highest PO Amount: =LARGE(I2:I81,3)
9. 2nd Lowest PO Amount: =SMALL(I2:I81,2)
10. 3rd Lowest PO Amount: =SMALL(I2:I81,3)


ANS .


<img width="3035" height="1909" alt="Picture 16" src="https://github.com/user-attachments/assets/121b5333-b417-4be3-b1b1-83cd1b90769a" />


Add calculated columns:
Col J — GST 18% Rounded to 2 decimals: =ROUND(I2*18%,2)
Col K — GST Rounded UP to nearest rupee: =ROUNDUP(I2*18%,0)
Col L — GST Rounded DOWN: =ROUNDDOWN(I2*18%,0)
Col M — Total with GST (using rounded): =I2+J2
Col N — Instalment 1 of 3 (round down): =ROUNDDOWN(I2/3,0)
Col O — Budget Variance ABS (budget=300000): =ABS(I2-300000)
Col P — PO Amount to nearest 1000 (FLOOR): =FLOOR(I2,1000)
Col Q — PO Amount rounded up to nearest 1000 (CEILING): =CEILING(I2,1000)
Col R — PO Amount to nearest 500 (MROUND): =MROUND(I2,500)

ANS . 


<img width="3149" height="1909" alt="Picture 17" src="https://github.com/user-attachments/assets/2ca7509e-894e-42ad-bd4c-0307634107a3" />


Revision tasks:
— Apply CF: PO Amount above 400000 = Red fill (revision)
— Sort by PO Amount Largest to Smallest (revision)
— Convert to table named "POAnalysis" (revision)

ANS . 


<img width="1895" height="747" alt="Screenshot 2026-07-16 201015" src="https://github.com/user-attachments/assets/0205b403-86a4-4d19-a55d-a6dbcb45efd0" />


<img width="3944" height="1909" alt="Picture 18" src="https://github.com/user-attachments/assets/46f4170d-2dfa-4190-bab4-3239cae37980" />



---


Hard Q2 — SAP Vendor Invoice GST Calculator 80 rows
This is a Vendor Invoice register. Complete all rounding and math tasks:

Add calculated columns:
Col I — CGST 9%: =ROUND(H2*9%,2)
Col J — SGST 9%: =ROUND(H2*9%,2)
Col K — IGST 18% (for interstate): =ROUND(H2*18%,2)
Col L — Total GST: =I2+J2
Col M — Invoice Total: =H2+L2
Col N — Invoice Total RoundUp: =ROUNDUP(M2,0)
Col O — Invoice Total RoundDown: =ROUNDDOWN(M2,0)
Col P — Invoice to nearest 100: =MROUND(M2,100)
Col Q — ABS Variance from 500000: =ABS(H2-500000)
Col R — Instalment 1 of 4: =ROUNDDOWN(M2/4,0)
Col S — MOD check (remainder when divided by 1000): =MOD(H2,1000)

Summary area below data:
1. Total Invoice Amount: SUM col H
2. Total GST collected: SUM col L
3. Total Payable: SUM col M
4. Average Invoice: AVERAGE col H
5. Highest Invoice: MAX col H
6. Lowest Invoice: MIN col H
7. 2nd Highest Invoice: LARGE(H,2)
8. 2nd Lowest Invoice: SMALL(H,2)
9. Total Entries: COUNTA col A
10. Count invoices with amount: COUNT col H

Revision tasks:
— CF: Invoice Total above 600000 = Red fill | below 200000 = Green fill (revision)
— Filter: State = Maharashtra → how many rows? (revision)
— Sort by Invoice Total largest to smallest (revision)


ANSWER :



Add calculated columns:
Col I — CGST 9%: =ROUND(H2*9%,2)
Col J — SGST 9%: =ROUND(H2*9%,2)
Col K — IGST 18% (for interstate): =ROUND(H2*18%,2)
Col L — Total GST: =I2+J2
Col M — Invoice Total: =H2+L2
Col N — Invoice Total RoundUp: =ROUNDUP(M2,0)
Col O — Invoice Total RoundDown: =ROUNDDOWN(M2,0)
Col P — Invoice to nearest 100: =MROUND(M2,100)
Col Q — ABS Variance from 500000: =ABS(H2-500000)
Col R — Instalment 1 of 4: =ROUNDDOWN(M2/4,0)
Col S — MOD check (remainder when divided by 1000): =MOD(H2,1000)

ANS . 


<img width="4176" height="1909" alt="Picture 19" src="https://github.com/user-attachments/assets/6d7c0eb1-d08d-49ad-915c-0485cd794359" />



Summary area below data:
1. Total Invoice Amount: SUM col H
2. Total GST collected: SUM col L
3. Total Payable: SUM col M
4. Average Invoice: AVERAGE col H
5. Highest Invoice: MAX col H
6. Lowest Invoice: MIN col H
7. 2nd Highest Invoice: LARGE(H,2)
8. 2nd Lowest Invoice: SMALL(H,2)
9. Total Entries: COUNTA col A
10. Count invoices with amount: COUNT col H


ANS .


<img width="4197" height="2109" alt="Picture 20" src="https://github.com/user-attachments/assets/c1fa5752-a9ba-4287-8eed-a214d0d6a8eb" />


Revision tasks:
— CF: Invoice Total above 600000 = Red fill | below 200000 = Green fill (revision)
— Filter: State = Maharashtra → how many rows? (revision)
— Sort by Invoice Total largest to smallest (revision)


ANS . 

— CF: Invoice Total above 600000 = Red fill | below 200000 = Green fill (revision)


<img width="4197" height="2135" alt="Picture 21" src="https://github.com/user-attachments/assets/2eae9d06-18fa-4df8-a34f-93da596bd2b6" />


— Filter: State = Maharashtra → how many rows? (revision)


<img width="4197" height="215" alt="Picture 22" src="https://github.com/user-attachments/assets/0191340a-917e-4775-a29d-ea75648d054b" />


— Sort by Invoice Total largest to smallest (revision)


<img width="4197" height="2135" alt="Picture 23" src="https://github.com/user-attachments/assets/7dd133a2-6207-406e-8db0-9139926d9927" />
