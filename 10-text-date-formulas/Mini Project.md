Mini Project — SAP PO Code Parsing & Aging Report 250 rows
Scenario: Your manager at Mahindra wants every PO ID broken into its parts (prefix, middle code, number) AND wants an aging report showing exactly how many working days each PO has been open. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "PO Code & Aging" (double-click tab)
2. In column K, use =LEFT(A2,2) to extract the "PO" prefix
3. In column L, use =MID(A2,FIND("-",A2)+1,2) to dynamically extract the middle code
4. In column M, use =VALUE(RIGHT(A2,4)) to extract the numeric PO number
5. In column N, use =PROPER(TRIM(C2)) to clean and properly capitalize every Vendor Name
6. In column O, use =NETWORKDAYS(B2,TODAY()) to calculate working days since order
7. In column P, use =IF(O2>30,"🔴 Aging Critical",IF(O2>15,"🟡 Watch","🟢 Fresh")) — combine Day 6-7 nested IF logic with today's date function
8. In column Q, use =EOMONTH(B2,0) to show which month-end each PO belongs to
9. Apply Conditional Formatting: Text Contains "Critical" on column P → Red Fill
10. Sort by column P using a Custom List (Critical, Watch, Fresh) so oldest problem POs group at the top
11. Add a Summary block starting S1: S1="Total Rows", T1=250; S2="Aging Critical POs", T2=count you observed; S3="Average Working Days Open", T3==AVERAGE(O2:O251)
12. Save using Ctrl+S, then Save As (F12) → name it: new-day-10-text-date-formulas-mahindra-po.xlsx
13. Create Sheet2 → rename "Text & Date Formula Log" → write down every formula used today
14. Bold and underline the header row (Day 1)
15. Turn on AutoFilter, filter Delivery Status = "Delayed" then clear (Day 2)
16. Select Qty column → Data Validation → Allow Whole Number → Between 1 and 100 (Day 3)
17. Use =VLOOKUP or INDEX+MATCH style thinking if a Vendor Master sheet is available (Day 9)



ANSWERS : 



<img width="2046" height="6277" alt="Picture 3" src="https://github.com/user-attachments/assets/0b0cc9e1-9a15-4e96-b797-3a72a877729a" />



<img width="2046" height="1902" alt="Picture 4" src="https://github.com/user-attachments/assets/9cca72e0-9c6f-4d97-baa3-947feef631c9" />


