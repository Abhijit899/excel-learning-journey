Business Question Answer in 1 line
A SAP MM consultant wants to flag a PO as "Needs Attention" if Delivery Status is EITHER "Delayed" OR "Pending" — either one is enough to flag it. .
Separately, they want a 3-tier PO Amount classification: "Low" under ₹50000, "Medium" ₹50000-₹200000, and "High" above ₹200000. Which two formula structures from today solve each part?


ANSWER : 


Use IF + OR for “Needs Attention” and Nested IF for the 3-tier PO Amount classification.




---



Hard Question — Full IF+OR & Nested IF Drill 220 rows · single combined question
Paste this data. Complete every task below in order, starting from column J:

1. In J2, use =OR(I2="Delayed",I2="Pending") to test both statuses together — observe the raw TRUE/FALSE result
2. In K2, use =IF(OR(I2="Delayed",I2="Pending"),"Needs Attention","On Track") — combine OR inside IF
3. In L2, use =IF(OR(H2>200000,F2="North"),"Review Required","Standard") — OR combining a number condition with a text condition
4. In M2, use =OR(F2="North",F2="South",F2="East") — a 3-condition OR test
5. In N2, use =IF(H2<50000,"Low",IF(H2<=200000,"Medium","High")) — a 3-tier nested IF classification
6. In O2, use =IF(H2<50000,"Low",IF(H2<=150000,"Medium",IF(H2<=300000,"High","Very High"))) — a 4-tier nested IF classification
7. In P2, combine everything: =IF(AND(H2>200000,I2="Delayed"),"Critical",IF(OR(I2="Delayed",I2="Pending"),"Watch","OK")) — reusing yesterday's AND alongside today's OR in one nested formula
8. Compare column K (IF+OR) against column J (a full-column count of TRUE from column O2's OR test) — confirm OR always matches equal or more rows than a single condition would
9. In Q1, write in words: what's the difference between using AND vs OR when checking two conditions?
10. Apply Conditional Formatting: Highlight Cells Rules → Text that Contains "Critical" on column P → Red Fill; "Watch" → Yellow Fill
11. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
12. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
13. Select Delivery Status column → Data Validation → Allow List → Delivered,Pending,Delayed (Day 3)
14. Apply a 3-Color Scale on PO Amount (Day 4)
15. Use =UNIQUE(A2:A221) to preview distinct PO IDs (Day 5)
16. Use =IF(AND(H2>200000,I2="Delayed"),"Priority","Normal") to re-confirm yesterday's IF+AND logic (Day 6)


ANSWER : 


<img width="1925" height="5527" alt="Picture 1" src="https://github.com/user-attachments/assets/ebd19664-cea7-4d97-a286-554e140dae51" />

