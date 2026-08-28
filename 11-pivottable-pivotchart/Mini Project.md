Mini Project — SAP Regional Spend Pivot Dashboard 250 rows
Scenario: Your manager at Mahindra wants a live dashboard sheet — Pivot Table plus chart — showing spend by Region and Category, that updates itself whenever new PO data is added. Complete all tasks:

1. Paste data in Sheet1 → rename to "PO Raw Data" → convert to a Table (Ctrl+T), name it "PO_Day11"
2. Insert a Pivot Table from this Table into a New Worksheet → rename that sheet "Spend Dashboard"
3. Build the Pivot Table: Region in Rows, Category in Columns, PO Amount in Values (Sum)
4. Add a 2nd Values field: Count of PO ID, so you see both total spend and number of POs per cell
5. Add Delivery Status to the Filters area
6. Group Order Date by Month in a separate area of Rows (or a second small Pivot Table) to see monthly spend trend
7. Insert a PivotChart (Clustered Column) showing Region totals
8. Insert a 2nd PivotChart (Pie) showing Category share of total spend
9. Go back to "PO Raw Data" → add 8 new rows below the Table → return to "Spend Dashboard" → Refresh All (Data tab → Refresh All) → confirm both charts update
10. Add a short Summary note in a blank cell on the dashboard: which Region has the highest spend, and which Category has the most POs, based on what you observed
11. Save using Ctrl+S, then Save As (F12) → name it: new-day-11-pivottable-pivotchart-mahindra-po.xlsx
12. Create a 3rd sheet → rename "Pivot Setup Log" → write down every field placement and grouping used today
13. Bold and underline the header row on "PO Raw Data" (Day 1)
14. Select Qty column → Data Validation → Allow Whole Number → Between 1 and 100 (Day 3)
15. Run Data → Remove Duplicates on PO ID, confirm none found (Day 5)
16. Use =IF(AND(H2>150000,I2="Delayed"),"Priority","Normal") on the raw data as a helper column (Day 6)
17. Use =NETWORKDAYS(B2,TODAY()) to show working days elapsed on the raw data (Day 10)



ANSWERS : 


<img width="1522" height="780" alt="Screenshot 2026-08-28 141658" src="https://github.com/user-attachments/assets/27791beb-dd23-40f6-8fdf-319d4928aed2" />


<img width="3631" height="193" alt="Picture 6" src="https://github.com/user-attachments/assets/0e831222-f579-4e62-beb0-0c87748de059" />


<img width="3637" height="505" alt="Picture 7" src="https://github.com/user-attachments/assets/71ac9852-67fc-4112-ada7-0b1d699e956e" />


<img width="1215" height="501" alt="Screenshot 2026-08-28 142207" src="https://github.com/user-attachments/assets/e9291343-98d4-444f-bc07-b5c72982e091" />


<img width="1183" height="493" alt="Screenshot 2026-08-28 142429" src="https://github.com/user-attachments/assets/e2c987cb-7be8-4478-a6de-0c0bc6df9423" />


<img width="1136" height="531" alt="Screenshot 2026-08-28 143620" src="https://github.com/user-attachments/assets/8b9dc426-af31-4541-8f2b-2acd23df921c" />


<img width="1513" height="621" alt="Screenshot 2026-08-28 143536" src="https://github.com/user-attachments/assets/f179caab-d56c-4684-983b-139ef38d51af" />


<img width="3209" height="2305" alt="Picture 9" src="https://github.com/user-attachments/assets/6c7d6399-b545-403f-9779-f0ce76889513" />


