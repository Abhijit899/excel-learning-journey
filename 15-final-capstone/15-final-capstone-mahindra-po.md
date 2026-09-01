Business Question Answer in 1 line
Your manager wants one button on the sheet that, when clicked, instantly formats the entire PO Amount column as Currency, bolds the header row, and freezes it — a repetitive task done every time new data arrives.
Which feature records this once and replays it forever with a single click?



ANSWERS : 







---



Section A — Navigation, Setup & Data Entry Day 1
1Rename Sheet1 to "PO Raw Data". Press Ctrl+End, confirm it lands on the true last cell (J321) — if not, clean the used range.
2Freeze the header row (View → Freeze Panes → Freeze Top Row).
3Select PO Amount → Ctrl+Shift+$ Currency format. Bold + underline the header row.


Section B — Sorting & Filtering Day 2
1Data → Sort → Level 1: Region (A-Z), Level 2: PO Amount (Largest to Smallest).
2Turn on AutoFilter (Ctrl+Shift+L) → filter Delivery Status="Delayed" AND Region="North" together → note the count → clear filters.
3Apply a Top 10 Number Filter on PO Amount, note the top vendors, then clear.


Section C — Advanced Filter & Data Validation Day 3
1Build a Criteria Range for Region="North" OR Delivery Status="Delayed" → Advanced Filter → Copy to a new area.
2Apply Data Validation: Delivery Status column → Allow List → Delivered,Pending,Delayed.
3Apply Data Validation: Qty column → Allow Whole Number → Between 0 and 100.


Section D — Conditional Formatting & Text Cleanup Day 4
1Select A2:J321 → New Rule → formula =$H2>200000 → Light Red Fill on entire row.
2Apply a 3-Color Scale on PO Amount and Data Bars on Qty.
3Ctrl+H → Find "Pend" → Replace "Pending" → Match Entire Cell Contents → Replace All.


Section E — Duplicates & Paste Special Day 5
1Use =UNIQUE(A2:A321) and =COUNTA(UNIQUE(A2:A321)) to preview distinct PO IDs before deleting anything.
2Run Data → Remove Duplicates on PO ID → confirm it matches your UNIQUE count (should remove 10).
3Type 1.08 → copy → Paste Special → Multiply on PO Amount for an 8% bulk price revision.


Section F — IF, AND, OR, Nested IF Day 6-7
1=IF(AND(H2>150000,I2="Delayed"),"🔴 Critical",IF(OR(I2="Delayed",I2="Pending"),"🟡 Watch","🟢 OK")) in a helper column.
2=IF(H2<50000,"Low",IF(H2<=200000,"Medium","High")) for a 3-tier amount classification.
3Apply Conditional Formatting: Text Contains "Critical" → Red Fill on that column.


Section G — SUMIF/COUNTIF/SUMIFS/COUNTIFS Day 8
1=SUMIFS(H2:H321,C2:C321,"North",I2:I321,"Delayed") — total for North+Delayed.
2=COUNTIFS(F2:F321,"Machinery",I2:I321,"Delayed") — count Machinery+Delayed.
3Build a small Region-wise spend summary table using SUMIF for each of the 4 regions.


Section H — MATCH/INDEX, VLOOKUP, HLOOKUP, XLOOKUP Day 9, 14
1=XLOOKUP(D2,'Vendor Master'!$A$2:$A$26,'Vendor Master'!$B$2:$B$26,"Not Found") — pull Vendor Name, fill down.
2=INDEX('Vendor Master'!$A$2:$A$26,MATCH(VendorName,'Vendor Master'!$B$2:$B$26,0)) — reverse lookup (Name→ID), proving VLOOKUP alone couldn't do this.
3=XLOOKUP(D2,'Vendor Master'!$A$2:$A$26,'Vendor Master'!$C$2:$C$26,"Not Found") — pull Payment Terms.


Section I — Text & Date Formulas Day 10
1=RIGHT(A2,4) then =VALUE(RIGHT(A2,4)) to extract the numeric PO number.
2=NETWORKDAYS(B2,TODAY()) for working days elapsed since order.
3=IF(NETWORKDAYS(B2,TODAY())>30,"Aging Critical","Fresh") combining both.


Section J — Pivot Table, Pivot Chart, Slicer, Timeline Day 11-12
1Convert cleaned data to a Table (Ctrl+T) → Insert PivotTable into a New Sheet "Dashboard".
2Region in Rows, Category in Columns, PO Amount in Values (Sum) + Count of PO ID as a 2nd Values field.
3Insert Slicers for Region and Delivery Status, insert a Timeline for Order Date, insert a PivotChart (Column).


Section K — Dynamic Arrays & Financial Functions Day 13
1=SORT(FILTER(A2:J321,(I2:I321="Delayed")*(H2:H321>150000)),8,-1) — live Delayed+high-value list, sorted.
2Build a Vendor Financing Calculator: Loan Amount, Rate, Term cells feeding =PMT(rate/12,term,-loan) for EMI.


Section L — Printing Day 14
1Set Print Area on the cleaned data, Print Titles to repeat row 1, Scale to Fit Width: 1 page.
2Ctrl+P → confirm headers repeat and layout fits cleanly across pages.


Section M — Macros (Today's New Skill) Day 15
1Enable the Developer tab (File → Options → Customize Ribbon → tick Developer).
2View → Macros → Record Macro → name it "FormatReport" → Store in This Workbook.
3While recording: select PO Amount → apply Currency format → select header row → Bold → Freeze Top Row → Stop Recording.
4Insert a Button shape on the sheet → Assign Macro → "FormatReport".
5Undo your manual formatting, then click the button — confirm it reapplies everything instantly.
6Save As → choose "Excel Macro-Enabled Workbook (*.xlsm)" — confirm this is required to keep the macro.


Section N — Final Summary & Wrap-Up
1Add a Summary block: Total Rows (320), Duplicates Removed (10), Unmatched Vendors (should be 0), Critical POs (count observed), Working Macro (Yes/No).
2Create a final sheet "Capstone Log" → write one line per Section (A-M) naming the feature used and what it accomplished.
3Save using Ctrl+S, then Save As (F12) → name it: new-day-15-final-capstone-mahindra-po.xlsm



ANSWERS : 


Section A — Navigation, Setup & Data Entry Day 1
1Rename Sheet1 to "PO Raw Data". Press Ctrl+End, confirm it lands on the true last cell (J321) — if not, clean the used range.
2Freeze the header row (View → Freeze Panes → Freeze Top Row).
3Select PO Amount → Ctrl+Shift+$ Currency format. Bold + underline the header row.


ANS . 


<img width="1293" height="672" alt="Screenshot 2026-09-01 205516" src="https://github.com/user-attachments/assets/afb00344-2840-40cb-848a-ba4b0a064659" />


<img width="1532" height="735" alt="Screenshot 2026-09-01 205605" src="https://github.com/user-attachments/assets/abd097b6-1e4a-493f-a818-299b2702c7ca" />



Section B — Sorting & Filtering Day 2
1Data → Sort → Level 1: Region (A-Z), Level 2: PO Amount (Largest to Smallest).
2Turn on AutoFilter (Ctrl+Shift+L) → filter Delivery Status="Delayed" AND Region="North" together → note the count → clear filters.
3Apply a Top 10 Number Filter on PO Amount, note the top vendors, then clear.


ANS . 


<img width="1160" height="7798" alt="Picture 3" src="https://github.com/user-attachments/assets/9c5a7399-604c-405b-b809-0b450015a4b1" />


<img width="1160" height="755" alt="Picture 4" src="https://github.com/user-attachments/assets/fbd230c9-e82e-4441-a65c-42b8da97a1a6" />


<img width="1407" height="412" alt="Screenshot 2026-09-01 210914" src="https://github.com/user-attachments/assets/c74e0099-549d-4253-99c0-2ea048caa8a4" />



Section C — Advanced Filter & Data Validation Day 3
1Build a Criteria Range for Region="North" OR Delivery Status="Delayed" → Advanced Filter → Copy to a new area.
2Apply Data Validation: Delivery Status column → Allow List → Delivered,Pending,Delayed.
3Apply Data Validation: Qty column → Allow Whole Number → Between 0 and 100.


ANS . 


<img width="2526" height="7800" alt="Picture 5" src="https://github.com/user-attachments/assets/252d1534-2177-4adb-b5f6-b07f89137000" />


<img width="1332" height="677" alt="Screenshot 2026-09-01 211356" src="https://github.com/user-attachments/assets/647dc0a0-9526-460b-b7fc-00753dee72c3" />


<img width="1236" height="670" alt="Screenshot 2026-09-01 211450" src="https://github.com/user-attachments/assets/2bf0c1dc-8a70-428c-b5b8-ff6068058f84" />


Section D — Conditional Formatting & Text Cleanup Day 4
1Select A2:J321 → New Rule → formula =$H2>200000 → Light Red Fill on entire row.
2Apply a 3-Color Scale on PO Amount and Data Bars on Qty.
3Ctrl+H → Find "Pend" → Replace "Pending" → Match Entire Cell Contents → Replace All.


ANS . 


<img width="1160" height="7800" alt="Picture 6" src="https://github.com/user-attachments/assets/f43cefc1-a402-4613-b3b4-173cd0540555" />


<img width="1160" height="7800" alt="Picture 7" src="https://github.com/user-attachments/assets/bca75622-214d-4933-bf97-a7092fbcced7" />


<img width="1527" height="682" alt="Screenshot 2026-09-01 212118" src="https://github.com/user-attachments/assets/2cd01aa2-e468-4ee4-b454-710a030e11b0" />

