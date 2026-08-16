Mini Project — SAP New PO Sheet Setup 250 rows
Scenario: Your manager at Mahindra hands you a completely fresh PO export with no calculations done yet. Set it up from scratch. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "PO Setup" (double-click the tab)
2. In column J, calculate PO Amount using =H2*I2, fill down to row 251
3. In column K, use =IF(J2>100000,"High Value","Normal") — a simple first look at conditional logic
4. Build a summary block starting L1: L1="Total PO Value", M1==SUM(J2:J251); L2="Average PO Amount", M2==AVERAGE(J2:J251); L3="Total Rows", M3=250
5. Apply Currency formatting (Ctrl+Shift+$) on column J
6. Bold and underline the header row using Ctrl+B then Ctrl+U
7. Use the Fill Handle to extend the PO ID series 10 more rows below the data
8. Freeze the header row so it stays visible while scrolling
9. Save using Ctrl+S, then Save As (F12) → name it: new-day-01-intro-basics-mahindra-po.xlsx
10. Create Sheet2 → rename "Formula Log" → write down every formula you used today with one line on what it does


ANSWERS : 


<img width="1389" height="6267" alt="Picture 8" src="https://github.com/user-attachments/assets/d29d52aa-403f-4a64-ad4a-d87c41691097" />
