Mini Project — SAP Live PO Tracker & Vendor Financing Calculator 250 rows
Scenario: Your manager at Mahindra wants a live-updating "Top Problem POs" list that needs zero manual maintenance, PLUS a quick calculator to check financing terms when a vendor requests an equipment advance. Complete all tasks:

1. Paste data in Sheet1 → rename to "PO Live Tracker" (double-click tab)
2. In a fresh area, use =SORT(FILTER(A2:I251,(I2:I251="Delayed")*(H2:H251>150000)),9,-1) — a live list of Delayed POs above ₹150000, sorted highest first (multiplying two conditions inside FILTER combines them with AND)
3. In another area, use =SORT(A2:I251,9,-1) for a full live-sorted list of every PO by Amount
4. Use =COUNTA(spill_range#) to count how many rows are in your Delayed+High-Value list
5. Build a small "Vendor Financing Calculator" section starting R1:
   R1="Loan Amount", S1=500000
   R2="Annual Rate", S2=9%
   R3="Term (Months)", S3=36
   R4="Monthly EMI", S4==PMT(S2/12,S3,-S1)
6. In S5, use =NPER(S2/12,-15000,S1) to show how many months it'd take at a fixed ₹15000/month payment instead
7. In S6, use =FV(S2/12,S3,-S4,S1) to confirm the loan reaches ₹0 balance after the calculated EMI over the full term (should return close to 0)
8. Change S1 to 750000 and confirm S4 (EMI) recalculates automatically — this is why building it with cell references instead of typed numbers matters
9. Add a Summary block starting U1: U1="Total Rows", V1=250; U2="Delayed+High-Value POs", V2=count you observed; U3="Monthly EMI (₹5L @ 9%, 3yr)", V3=value you observed
10. Save using Ctrl+S, then Save As (F12) → name it: new-day-13-dynamicarrays-financial-mahindra-po.xlsx
11. Create Sheet2 → rename "Dynamic Array & Finance Log" → write down every formula used today
12. Bold and underline the header row (Day 1)
13. Select Qty column → Data Validation → Allow Whole Number → Between 1 and 100 (Day 3)
14. Run Data → Remove Duplicates on PO ID, confirm none found (Day 5)
15. Use =IF(AND(H2>150000,I2="Delayed"),"Priority","Normal") as a helper column (Day 6)
16. Insert a Slicer on a quick Pivot Table built from this data (Day 12)



ANSWERS : 


<img width="872" height="427" alt="Screenshot 2026-08-31 133258" src="https://github.com/user-attachments/assets/201b4478-0721-448f-a382-a6ca05b3dad8" />


<img width="2058" height="6027" alt="Picture 1" src="https://github.com/user-attachments/assets/cfb8ff1d-11a8-4b59-be94-0321631c9784" />


<img width="1513" height="650" alt="Screenshot 2026-08-31 133531" src="https://github.com/user-attachments/assets/598e1f76-1893-4193-9e52-03c32b5bd41e" />


<img width="1331" height="6027" alt="Picture 2" src="https://github.com/user-attachments/assets/f0aceb76-99dc-4eaa-826f-dd9636dc6032" />


<img width="1518" height="697" alt="Screenshot 2026-08-31 133929" src="https://github.com/user-attachments/assets/cfbe33d1-12d9-4b4d-999e-bf642f5b4f88" />
