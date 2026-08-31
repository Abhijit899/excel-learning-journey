Business Question Answer in 1 line
You have a tiny Region→HQ City table where Region sits in the LEFT column and HQ City in the RIGHT column. Your manager now asks the OPPOSITE question: "which Region does Chennai belong to?" — the answer column is now to the LEFT of what you'd search. VLOOKUP cannot do this directly. Which two functions, combined, solve it?


ANSWER : 


INDEX + MATCH 


---




Hard Question — Full MATCH/INDEX & VLOOKUP/HLOOKUP Drill 220 rows · ONE single dataset
Paste this data into A1 of Sheet1. Everything you need is in this one table — Vendor Name is already included. Complete every task below in order, starting from column K:

Type these two tiny tables directly into a spare area (no separate paste needed):
Region HQ table (type in M1:N5): M1="Region",N1="HQ City" / M2="North",N2="Delhi" / M3="South",N3="Chennai" / M4="East",N4="Kolkata" / M5="West",N5="Mumbai"
Category Discount table (type in M7:U8, horizontal): M7="Category" with the 8 category names across N7:U7 (Raw Material, Packaging, Machinery, Chemicals, IT Equipment, Office Supplies, Logistics, Utilities), and discount % values 5,3,8,6,4,2,7,5 across N8:U8

MATCH & INDEX basics:
1. In K1, use =MATCH("South",$M$2:$M$5,0) to find South's position — confirm it returns 2
2. In K2, use =INDEX($N$2:$N$5,K1) to return the HQ City at that position — confirm it shows "Chennai"
3. In L2, combine both into ONE formula: =INDEX($N$2:$N$5,MATCH(E2,$M$2:$M$5,0)), fill down to L221 — pulls HQ City using each row's Region
4. In N1, type "Chennai" → in N2, go the OPPOSITE direction (impossible with VLOOKUP): =INDEX($M$2:$M$5,MATCH(N1,$N$2:$N$5,0)) — looks up Region USING HQ City
VLOOKUP & HLOOKUP:
5. In O2, use =VLOOKUP(E2,$M$2:$N$5,2,FALSE) to pull HQ City the VLOOKUP way, fill down — compare against L2's result
6. In P2, use =HLOOKUP(F2,$M$7:$U$8,2,FALSE) to pull each row's Category discount %, fill down
Error handling & reflection:
7. In Q2, wrap task 3's formula in IFERROR: =IFERROR(INDEX($N$2:$N$5,MATCH(E2,$M$2:$M$5,0)),"Region Not Found")
8. In R1, write in words: why can INDEX+MATCH look LEFT (Region from HQ) while VLOOKUP cannot?
9. In R2, write in words: when would you use HLOOKUP instead of VLOOKUP
10. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
11. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
12. Apply a 3-Color Scale on PO Amount (Day 4)
13. Use =IF(AND(H2>200000,I2="Delayed"),"Priority","Normal") (Day 6)
14. Use =SUMIFS(H2:H221,C2:C221,"North",I2:I221,"Delayed") — total for North+Delayed (Day 8)


ANSWERS : 


