Business Question Answer in 1 line
A SAP MM consultant needs the TOTAL PO Amount specifically for North region AND Delayed status only — not the whole sheet's total. 
Which single function handles two conditions at once, and in what order do its arguments go compared to the single-condition version?



ANSWER : 

=SUMIFS 






---



Hard Question — Full SUMIF/COUNTIF/SUMIFS/COUNTIFS Drill 220 rows · single combined question
Paste this data. Complete every task below in order, starting from column K:

Single-condition:
1. In K1, use =SUMIF(F2:F221,"North",H2:H221) to total PO Amount for North region only
2. In K2, use =COUNTIF(I2:I221,"Delayed") to count how many POs are Delayed
3. In K3, use =SUMIF(H2:H221,">200000") to total only PO Amounts greater than 200000
4. In K4, use =COUNTIF(C2:C221,"*Steel*") to count vendors with "Steel" in the name
5. In K5, use =SUMIF(C2:C221,"*Steel*",H2:H221) to total PO Amount for those same Steel vendors
Multi-condition:
6. In K6, use =SUMIFS(H2:H221,F2:F221,"North",I2:I221,"Delayed") — total for North+Delayed together
7. In K7, use =COUNTIFS(F2:F221,"West",G2:G221,"IT Equipment") — count West+IT Equipment
8. In K8, use =SUMIFS(H2:H221,I2:I221,"Delayed",H2:H221,">150000") — Delayed POs that are ALSO above 150000
9. In K9, use =COUNTIFS(F2:F221,"North",F2:F221,"South") and confirm it returns 0 — a row can't match two different regions at once
Dynamic & reflect:
10. Add helper cells M1="North", N1="Delayed" → in K10 use =SUMIFS(H2:H221,F2:F221,M1,I2:I221,N1) — change M1/N1 and confirm K10 updates automatically
11. In P1, write in words: why does SUMIFS put sum_range FIRST while SUMIF puts sum_range LAST?
12. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
13. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
14. Select Delivery Status column → Data Validation → Allow List → Delivered,Pending,Delayed (Day 3)
15. Apply a 3-Color Scale on PO Amount (Day 4)
16. Use =UNIQUE(A2:A221) to preview distinct PO IDs (Day 5)
17. Use =IF(AND(H2>200000,I2="Delayed"),"Priority","Normal") (Day 6)
18. Use =IF(OR(I2="Delayed",I2="Pending"),"Needs Attention","On Track") (Day 7)


ANSWERS : 


<img width="2324" height="5528" alt="Picture 3" src="https://github.com/user-attachments/assets/7e1c6760-8805-444f-8de8-52522c240f8b" />



<img width="2324" height="5528" alt="Picture 4" src="https://github.com/user-attachments/assets/105d6024-c269-4151-bad5-2c652abeee83" />


