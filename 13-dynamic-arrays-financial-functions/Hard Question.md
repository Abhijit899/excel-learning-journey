Business Question Answer in 1 line
A SAP MM consultant needs a LIVE, self-updating list of POs sorted by Amount (highest first), showing ONLY the Delayed ones — 
no Pivot Table, no manual re-filtering when new rows are added. Separately, Finance wants the monthly EMI for a ₹5,00,000 equipment loan at 9% annual interest over 3 years. Which function solves the first problem, and which solves the second?



ANSWERS : 


SORT + FILTER AND PMT 

---



Hard Question — Full Dynamic Array & Financial Function Drill 220 rows · single combined question
Paste this data. Complete every task below in order, starting from column K:

Dynamic Arrays:
1. In K1, use =SORT(A2:I221,9,-1) to create a LIVE full-table sort by PO Amount, highest first — confirm it spills down automatically
2. In a fresh area (T1), use =FILTER(A2:I221,I2:I221="Delayed") to create a LIVE list of only Delayed POs
3. In a fresh area (AC1), combine both: =SORT(FILTER(A2:I221,I2:I221="Delayed"),9,-1) — a live, filtered, AND sorted list in one formula
4. Add =FILTER(A2:I221,I2:I221="Delayed","No Delayed POs Found") to test the if_empty argument by temporarily changing the condition to something that matches nothing, then change it back
5. Use =SORTBY(C2:C221,H2:H221,-1) to sort Vendor Names by their PO Amount (a column not even shown in the output)
6. Reference the spill range from task 1 using =COUNTA(K1#) to count how many rows spilled
7. Go to your raw data → add 3 new rows below row 221 → confirm your FILTER/SORT formulas from tasks 1-3 automatically include the new rows without any changes needed
Financial Functions:
8. In AJ1, use =PMT(9%/12,36,-500000) to calculate the monthly EMI on a ₹5,00,000 equipment loan at 9% annual interest over 3 years
9. In AJ2, use =FV(6%/12,60,-5000) to calculate the future value of saving ₹5000/month at 6% annual interest over 5 years
10. In AJ3, use =PV(8%/12,24,-10000) to calculate the present value of receiving ₹10000/month for 2 years at 8% annual interest
11. In AJ4, use =NPER(9%/12,-15000,500000) to calculate how many months it takes to pay off the same ₹5,00,000 loan if paying ₹15000/month
12. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
13. Apply a 3-Color Scale on PO Amount (Day 4)
14. Use =SUMIFS(H2:H221,E2:E221,"North",I2:I221,"Delayed") and compare against your FILTER result count (Day 8)
15. Use =INDEX/MATCH style thinking to confirm Vendor ID patterns (Day 9)
16. Build a quick Pivot Table on this same data and insert a Slicer for Region (Day 11-12)



ANSWERS : 


<img width="1476" height="667" alt="Screenshot 2026-08-30 114719" src="https://github.com/user-attachments/assets/6ba6c3e1-b8b1-4604-ab2b-e036f87d43a6" />


<img width="1253" height="637" alt="Screenshot 2026-08-30 115203" src="https://github.com/user-attachments/assets/d2a7bfbc-cdd2-46d3-9ba3-b63378d49c25" />


<img width="1347" height="702" alt="Screenshot 2026-08-30 115704" src="https://github.com/user-attachments/assets/9ee7eb68-ad5c-438a-82e9-0fcb0c1e96bc" />


<img width="1290" height="5331" alt="Picture 2" src="https://github.com/user-attachments/assets/04597a50-7132-4223-b031-2f192138e199" />


<img width="1353" height="717" alt="Screenshot 2026-08-30 120246" src="https://github.com/user-attachments/assets/d2a7e78f-3934-430d-84fb-a3f7095b5a75" />


