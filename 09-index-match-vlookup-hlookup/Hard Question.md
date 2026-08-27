Business Question Answer in 1 line
A SAP MM consultant's Vendor Master table has Vendor Name in column A and Vendor ID in column B — but they need to look up Vendor ID USING Vendor Name (the answer column is to the LEFT of where VLOOKUP would need it). 
VLOOKUP cannot do this directly. Which two functions, combined, solve it?


ANSWER : 


INDEX + MATCH



---



Hard Question — Full MATCH/INDEX & VLOOKUP/HLOOKUP Drill 220 rows · single combined question
Paste this data in Sheet1. Complete every task below in order, starting from column J:

MATCH & INDEX basics:
1. In J1, use =MATCH("V-010",'Lookup Tables'!$A$2:$A$26,0) to find V-010's position in Vendor Master — confirm it returns 10
2. In J2, use =INDEX('Lookup Tables'!$B$2:$B$26,J1) to return the Vendor Name at that position — confirm it matches V-010's actual vendor
3. In K2, combine both into ONE formula: =INDEX('Lookup Tables'!$B$2:$B$26,MATCH(D2,'Lookup Tables'!$A$2:$A$26,0)), fill down to K221 — this pulls Vendor Name using Vendor ID, same result as VLOOKUP would give
4. In L2, now go the OPPOSITE direction (impossible with VLOOKUP): =INDEX('Lookup Tables'!$A$2:$A$26,MATCH(K2,'Lookup Tables'!$B$2:$B$26,0)) — looks up Vendor ID USING Vendor Name, fill down
VLOOKUP & HLOOKUP:
5. In M2, use =VLOOKUP(D2,'Lookup Tables'!$A$2:$D$26,3,FALSE) to pull Payment Terms using Vendor ID, fill down
6. In N2, use =VLOOKUP(D2,'Lookup Tables'!$A$2:$D$26,4,FALSE) to pull Region HQ, fill down
7. In O2, use =HLOOKUP(G2,'Lookup Tables'!$A$30:$I$31,2,FALSE) to pull each row's Category discount % from the horizontal table, fill down
Error handling & reflection:
8. In P2, wrap task 3's formula in IFERROR: =IFERROR(INDEX('Lookup Tables'!$B$2:$B$26,MATCH(D2,'Lookup Tables'!$A$2:$A$26,0)),"Vendor Not Found")
9. In Q1, write in words: why can INDEX+MATCH look LEFT while VLOOKUP cannot?
10. In Q2, write in words: when would you use HLOOKUP instead of VLOOKUP?
11. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
12. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
13. Apply a 3-Color Scale on PO Amount (Day 4)
14. Use =IF(AND(H2>200000,I2="Delayed"),"Priority","Normal") (Day 6)
15. Use =SUMIFS(H2:H221,C2:C221,"North",I2:I221,"Delayed") — total for North+Delayed (Day 8)


ANSWERS : 

