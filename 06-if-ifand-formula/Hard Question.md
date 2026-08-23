**Business Question Answer in 1 line**

A SAP MM consultant needs to mark a PO as "Priority" only if PO Amount is above ₹200000 AND Delivery Status is "Delayed" — not if only one of those two is true. Which exact formula structure, combining two functions from today, solves this correctly?   if + AND Formula 


ANSWER : 


Use IF + AND — =IF(AND(PO Amount>200000,Delivery Status="Delayed"),"Priority","").




---



Hard Question — Full IF & IF+AND Drill 220 rows · single combined question
Paste this data. Complete every task below in order, starting from column J:

1. In J2, use =IF(H2>200000,"High Value","Normal") to classify by PO Amount alone, fill down to J221
2. In K2, use =IF(I2="Delayed","Flag","OK") to classify by Delivery Status alone
3. In L2, use =IF(H2>=100000,"Above 1L","Below 1L") to practice the >= operator
4. In M2, use =IF(I2<>"Delivered","Not Yet Delivered","Delivered") to practice the <> (not equal) operator
5. In N2, use =IF(H2>200000,"High Value","") so the cell shows nothing (blank) instead of "Normal" when false
6. In O2, use =AND(H2>200000,I2="Delayed") to test both conditions together — observe the raw TRUE/FALSE result
7. In P2, use =IF(AND(H2>200000,I2="Delayed"),"Priority","Normal") — combine AND inside IF for the real decision
8. In Q2, use =IF(AND(H2>200000,I2="Delayed",G2="Machinery"),"Critical Machinery PO","Normal") — a 3-condition AND test
9. Compare column J (single IF) against column P (IF+AND) — count how many rows say "High Value" in J vs "Priority" in P, and explain in R1 why P's count is smaller
10. Apply Conditional Formatting: Highlight Cells Rules → Text that Contains "Priority" on column P → Red Fill
11. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
12. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
13. Select Delivery Status column → Data Validation → Allow List → Delivered,Pending,Delayed (Day 3)
14. Apply a 3-Color Scale on PO Amount (Day 4)
15. Use =UNIQUE(A2:A221) to preview distinct PO IDs (Day 5)



ANSWER : 


<img width="1848" height="5536" alt="Picture 45" src="https://github.com/user-attachments/assets/7f03bb53-a650-4b14-928a-bccdb7fea0be" />


<img width="1848" height="5536" alt="Picture 46" src="https://github.com/user-attachments/assets/bdbf3dea-fcad-44ea-8770-0f6225db9ab9" />


<img width="2007" height="5527" alt="Picture 47" src="https://github.com/user-attachments/assets/0885e60c-719e-48e2-9370-7dbecb207363" />

