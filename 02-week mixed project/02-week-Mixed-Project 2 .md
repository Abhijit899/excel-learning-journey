Scenario: You are a junior SAP MM consultant at Mahindra & Mahindra. It is month-end. Your manager gives you a raw 150-row PO dump exported from SAP and says:

"Clean it, format it professionally, add calculations, flag all issues, sort by priority, and give me a summary sheet. I need this in 2 hours."

This is your Week 1 final test. Every skill you learned this week must be used in this one file.


Step by Step Tasks — Complete in Order

STEP 1 — Data Entry & Fill Series
1. Paste data in Sheet 1 — rename sheet to "PO Data"
2. Add column A called "Sr No" — use Fill Series to number 1 to 150
3. Add column B called "FY" — type FY2026-27 in B2 → fill down to B151 using Ctrl+D
(shift existing columns right to make room — right click column A → Insert → repeat for B)


STEP 2 — Find & Replace (clean the errors)
Open Ctrl+H for each:
— Find "Dlyd" → Replace "Delayed" (Delivery Status)
— Find "Pndg" → Replace "Pending" (Delivery Status)
— Find "Dlvd" → Replace "Delivered" (Delivery Status)
— Find "Pd" → Replace "Paid" → tick Match Entire Cell Contents before replacing
— Find "Ovrd" → Replace "Overdue" → tick Match Entire Cell Contents
— Find "Tata Steeel" → Replace "Tata Steel"
— Find "Reliance Indstries" → Replace "Reliance Industries"


STEP 3 — Go To Special (fix blank cells)
1. Select PO Amount column → Ctrl+G → Special → Blanks → type 0 → Ctrl+Enter
2. Select Delivery Status column → Ctrl+G → Special → Blanks → type Pending → Ctrl+Enter
3. Select Payment Status column → Ctrl+G → Special → Blanks → type Pending → Ctrl+Enter


STEP 4 — Convert to Table
1. Click anywhere in data → Ctrl+T → tick My table has headers → OK
2. Rename table to "MahindraPO" in Table Design tab
3. Apply Table Style Medium 9 (dark blue)
4. Enable Total Row


STEP 5 — Rate Setup (outside table)
In cols P and Q (outside table):
P1 = GST Rate    Q1 = 18%
P2 = Budget      Q2 = 400000
P3 = Discount    Q3 = 2%


STEP 6 — Add Calculated Columns (Cell Referencing)
Add these columns inside the table — type formula in first data row only, table fills rest automatically:

Col L — GST Amount: =[@[PO Amount]]*$Q$1
Col M — Total with GST: =[@[PO Amount]]+[@[GST Amount]]
Col N — Budget Variance: =[@[PO Amount]]-$Q$2
Col O — Discount: =[@[Total with GST]]*$Q$3
Col P — Final Payable: =[@[Total with GST]]-[@[Discount]]
Col Q — Rounded Final: =ROUND([@[Final Payable]],0)

Note: your rate setup (P and Q) will shift — move rate setup to cols S and T after table columns are added



STEP 7 — Number Formatting
1. PO Amount column → Accounting format ₹ 2 decimals
2. GST Amount column → Accounting format ₹
3. Total with GST → Accounting format ₹
4. Final Payable → Accounting format ₹
5. Order Date column → DD-MMM-YYYY format
6. Header row → Bold, Dark Blue background, White font


STEP 8 — Conditional Formatting
1. Delivery Status = Delayed → Orange fill entire row: =$K2="Delayed"
2. Delivery Status = Pending → Yellow fill entire row: =$K2="Pending"
3. Delivery Status = Delivered → Green fill entire row: =$K2="Delivered"
4. Payment Status = Overdue → Red font entire row: =$L2="Overdue"
5. Budget Variance positive (over budget) → Bold Red font on Budget Variance column
6. Final Payable above 600000 → Red fill on Final Payable column
7. Apply Color Scale on PO Amount column (Green=high, Red=low)
8. Apply Data Bars on Qty column


STEP 9 — Sorting
Multi-level sort:
Level 1 → Payment Status → Custom Order: Overdue → Pending → Paid
Level 2 → Final Payable → Largest to Smallest


STEP 10 — Filter & Extract
1. Filter Delivery Status = Delayed AND Payment Status = Overdue
2. Go To Special → Visible Cells Only → Copy
3. Paste into Sheet 3 named "Escalation List" → Paste Special → Values + Formats
4. Clear filter in PO Data sheet


STEP 11 — Summary Sheet
Create Sheet 2 named "Summary Dashboard" — all values using structured references only:

Label in col A → Formula in col B:
Total PO Amount → =SUM(MahindraPO[PO Amount])
Total GST → =SUM(MahindraPO[GST Amount])
Total Final Payable → =SUM(MahindraPO[Final Payable])
Average PO Amount → =AVERAGE(MahindraPO[PO Amount])
Highest PO → =MAX(MahindraPO[PO Amount])
Lowest PO → =MIN(MahindraPO[PO Amount])
Total Entries → =COUNTA(MahindraPO[PO ID])
GST Rate → ='PO Data'!T1
Budget per PO → ='PO Data'!T2

Format Summary sheet professionally — bold headers, borders, accounting format on amounts


STEP 12 — Final Checks
1. Clear all filters in PO Data sheet
2. Clear any stray formatting in empty columns beyond Q
3. Freeze top row in PO Data sheet (View → Freeze Panes → Freeze Top Row)
4. Set Print Area on PO Data sheet → Landscape → Fit width to 1 page → Print Titles Row 1
5. Save as: week1-mixed-project-mahindra-po-report.xlsx


ANSWERS :



STEP 1 — Data Entry & Fill Series
1. Paste data in Sheet 1 — rename sheet to "PO Data"
2. Add column A called "Sr No" — use Fill Series to number 1 to 150
3. Add column B called "FY" — type FY2026-27 in B2 → fill down to B151 using Ctrl+D
(shift existing columns right to make room — right click column A → Insert → repeat for B)

ANS. 


<img width="1407" height="3627" alt="Picture 4" src="https://github.com/user-attachments/assets/6152efc1-a346-43ca-9554-ac6e0cff96af" />



STEP 2 — Find & Replace (clean the errors)
Open Ctrl+H for each:
— Find "Dlyd" → Replace "Delayed" (Delivery Status)
— Find "Pndg" → Replace "Pending" (Delivery Status)
— Find "Dlvd" → Replace "Delivered" (Delivery Status)
— Find "Pd" → Replace "Paid" → tick Match Entire Cell Contents before replacing
— Find "Ovrd" → Replace "Overdue" → tick Match Entire Cell Contents
— Find "Tata Steeel" → Replace "Tata Steel"
— Find "Reliance Indstries" → Replace "Reliance Industries"


ANS. 


<img width="1407" height="3627" alt="Picture 5" src="https://github.com/user-attachments/assets/0eebdad3-66c4-449d-ad6a-ddee8c79ae05" />



STEP 3 — Go To Special (fix blank cells)
1. Select PO Amount column → Ctrl+G → Special → Blanks → type 0 → Ctrl+Enter
2. Select Delivery Status column → Ctrl+G → Special → Blanks → type Pending → Ctrl+Enter
3. Select Payment Status column → Ctrl+G → Special → Blanks → type Pending → Ctrl+Enter


ANS . 


<img width="1407" height="3627" alt="Picture 6" src="https://github.com/user-attachments/assets/85b4467f-ff2e-4ff1-8180-8073294b5d4d" />



STEP 4 — Convert to Table
1. Click anywhere in data → Ctrl+T → tick My table has headers → OK
2. Rename table to "MahindraPO" in Table Design tab
3. Apply Table Style Medium 9 (dark blue)
4. Enable Total Row


ANS. 


<img width="1130" height="859" alt="Screenshot 2026-07-15 122923" src="https://github.com/user-attachments/assets/3042ded3-9d56-4c76-8460-ae25e0fde4e7" />


STEP 5 — Rate Setup (outside table)
In cols P and Q (outside table):
P1 = GST Rate    Q1 = 18%
P2 = Budget      Q2 = 400000
P3 = Discount    Q3 = 2%

ANS. 


<img width="1974" height="3655" alt="Picture 7" src="https://github.com/user-attachments/assets/b6fe7823-8c50-4c5b-869d-f26ef4c8b645" />



STEP 6 — Add Calculated Columns (Cell Referencing)
Add these columns inside the table — type formula in first data row only, table fills rest automatically:

Col L — GST Amount: =[@[PO Amount]]*$Q$1
Col M — Total with GST: =[@[PO Amount]]+[@[GST Amount]]
Col N — Budget Variance: =[@[PO Amount]]-$Q$2
Col O — Discount: =[@[Total with GST]]*$Q$3
Col P — Final Payable: =[@[Total with GST]]-[@[Discount]]
Col Q — Rounded Final: =ROUND([@[Final Payable]],0)


ANS .


<img width="2598" height="3655" alt="Picture 8" src="https://github.com/user-attachments/assets/784a0483-3bda-48b1-9e25-e4201047e8fc" />


STEP 7 — Number Formatting
1. PO Amount column → Accounting format ₹ 2 decimals
2. GST Amount column → Accounting format ₹
3. Total with GST → Accounting format ₹
4. Final Payable → Accounting format ₹
5. Order Date column → DD-MMM-YYYY format
6. Header row → Bold, Dark Blue background, White font

ANS. 


<img width="2608" height="3639" alt="Picture 9" src="https://github.com/user-attachments/assets/27215c63-b605-4218-9d56-97d59968c474" />



STEP 8 — Conditional Formatting
1. Delivery Status = Delayed → Orange fill entire row: =$K2="Delayed"
2. Delivery Status = Pending → Yellow fill entire row: =$K2="Pending"
3. Delivery Status = Delivered → Green fill entire row: =$K2="Delivered"
4. Payment Status = Overdue → Red font entire row: =$L2="Overdue"
5. Budget Variance positive (over budget) → Bold Red font on Budget Variance column
6. Final Payable above 600000 → Red fill on Final Payable column
7. Apply Color Scale on PO Amount column (Green=high, Red=low)
8. Apply Data Bars on Qty column

ANS .


<img width="2608" height="3639" alt="Picture 10" src="https://github.com/user-attachments/assets/c0d1bae2-1075-4f45-a5d4-2394a3f7255c" />


STEP 9 — Sorting
Multi-level sort:
Level 1 → Payment Status → Custom Order: Overdue → Pending → Paid
Level 2 → Final Payable → Largest to Smallest


ANS .


<img width="2608" height="3639" alt="Picture 14" src="https://github.com/user-attachments/assets/a6d69ad7-eafa-4d38-b41f-dbdf9dafdcd8" />



STEP 10 — Filter & Extract
1. Filter Delivery Status = Delayed AND Payment Status = Overdue
2. Go To Special → Visible Cells Only → Copy
3. Paste into Sheet 3 named "Escalation List" → Paste Special → Values + Formats
4. Clear filter in PO Data sheet


ANS.


<img width="2130" height="1100" alt="Picture 15" src="https://github.com/user-attachments/assets/f67ccb4b-8700-4444-b280-3705a98fc1bf" />



STEP 11 — Summary Sheet
Create Sheet 2 named "Summary Dashboard" — all values using structured references only:

Label in col A → Formula in col B:
Total PO Amount → =SUM(MahindraPO[PO Amount])
Total GST → =SUM(MahindraPO[GST Amount])
Total Final Payable → =SUM(MahindraPO[Final Payable])
Average PO Amount → =AVERAGE(MahindraPO[PO Amount])
Highest PO → =MAX(MahindraPO[PO Amount])
Lowest PO → =MIN(MahindraPO[PO Amount])
Total Entries → =COUNTA(MahindraPO[PO ID])
GST Rate → ='PO Data'!T1
Budget per PO → ='PO Data'!T2


ANS. 



<img width="786" height="393" alt="Screenshot 2026-07-15 133532" src="https://github.com/user-attachments/assets/ae419bcf-f8ec-4634-8c0b-4f463d517385" />








