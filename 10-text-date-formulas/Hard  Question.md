Business Question Answer in 1 line
A SAP MM consultant has PO IDs like "PO-MM-1001" and needs to extract just the numeric part (1001) for sorting. They also need to know exactly how many WORKING days have passed since each PO's Order Date, excluding weekends. 
Which text function combo extracts the number, and which single date function counts only working days?


ANSWER : 






---



Hard Question — Full Text & Date Formula Drill 220 rows · single combined question
Paste this data. Notice some Vendor Names have extra spaces on purpose. Complete every task below in order, starting from column J:

Text Formulas:
1. In J2, use =RIGHT(A2,4) to extract the last 4 digits of the PO ID as text, fill down to J221
2. In K2, use =VALUE(RIGHT(A2,4)) to convert that extracted text into a real number
3. In L2, use =FIND("-",A2) to find the position of the FIRST dash in the PO ID, then in M2 use =MID(A2,FIND("-",A2)+1,2) to dynamically extract the middle code ("MM")
4. In N2, use =LEN(C2) to check Vendor Name length, then in O2 use =TRIM(C2) and =LEN(TRIM(C2)) in P2 to compare original vs cleaned length
5. In Q2, use =UPPER(C2) and in R2 use =PROPER(TRIM(C2)) to clean AND capitalize properly in one step
6. In S2, use =TEXTJOIN(" | ",TRUE,E2,F2,G2) to combine Region, State, Category into one label
Date Formulas:
7. In T2, use =DAY(B2), U2 use =MONTH(B2), V2 use =YEAR(B2) to split Order Date into 3 parts
8. In W2, use =TODAY()-B2 to calculate total calendar days since order
9. In X2, use =NETWORKDAYS(B2,TODAY()) to calculate WORKING days only since order
10. In Y2, use =DATEDIF(B2,TODAY(),"D") to confirm it matches W2's result using a different function
11. In Z2, use =EDATE(B2,6) to calculate a 6-month check-in date from the order date
12. In AA2, use =EOMONTH(B2,0) to find the last day of the order's month
13. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
14. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
15. Apply a 3-Color Scale on PO Amount (Day 4)
16. Use =SUMIFS(H2:H221,E2:E221,"North",I2:I221,"Delayed") (Day 8)
17. Use =INDEX/MATCH or VLOOKUP style thinking to confirm PO ID prefix pattern makes sense across rows (Day 9)



ANSWER : 



<img width="2461" height="5527" alt="Picture 1" src="https://github.com/user-attachments/assets/01c85435-478d-4e50-96db-df35ccb9b4a5" />



<img width="3315" height="5527" alt="Picture 2" src="https://github.com/user-attachments/assets/97de93ff-790a-44ba-9bea-175935052722" />



