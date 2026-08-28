<img width="1527" height="695" alt="Screenshot 2026-08-28 135107" src="https://github.com/user-attachments/assets/ce8dab2c-18ed-4af7-9f22-a56e90e22bf1" /><img width="4812" height="529" alt="Picture 5" src="https://github.com/user-attachments/assets/64bd7b93-6632-477c-a1cf-2feb34db5f27" />Business Question Answer in 1 line
A SAP MM consultant needs to see Total PO Amount broken down by Region AND Category in a cross-tab layout, with the ability to instantly switch between Sum, Count, or Average — without writing a single SUMIFS formula.
Which single feature does all of this, and what's it called once turned into a visual?



ANSWER : 


Pivot Table → Analyze/Summarize data
Pivot Chart → Visualize that Pivot Table




---

Hard Question — Full Pivot Table & Pivot Chart Drill 220 rows · single combined question
Paste this data in Sheet1. Convert it to a Table first (Ctrl+T) so the Pivot Table can auto-expand later. Complete every task below in order:

1. Select any cell in the Table → Insert → PivotTable → New Worksheet → OK
2. Drag Region into Rows, Category into Columns, PO Amount into Values (defaults to Sum) — confirm you see a cross-tab of totals
3. Right-click any value in the Pivot Table → Value Field Settings → change from Sum to Average — observe every number change
4. Change it again to Count — confirm it now shows how many POs, not a money value
5. Change it back to Sum for the rest of the tasks
6. Drag Delivery Status into the Filters area — use the filter dropdown to show only "Delayed" POs, then switch back to "(All)"
7. Drag Order Date into Rows below Region → right-click a date → Group → select Months — confirm dates now group by month instead of showing every individual date
8. Add PO ID into Values a 2nd time → change its Value Field Settings to Count — now your Pivot Table shows both Sum of PO Amount AND Count of PO ID together
9. Go back to your raw data sheet, add 5 new rows below the Table (they should auto-join the Table since it's Ctrl+T formatted) → return to the Pivot Table → right-click → Refresh → confirm the totals updated
10. Select any cell in the Pivot Table → PivotTable Analyze tab → PivotChart → choose Clustered Column → OK
11. Change the chart type to Pie (right-click chart → Change Chart Type → Pie) → observe how Region totals now show as a share of the whole
12. Use the Field Buttons on the chart itself to filter by Region directly, without touching the Pivot Table
13. Use the Name Box to jump directly to K1 on your raw data sheet, then Ctrl+Home back to A1 (Day 1)
14. Data → Sort → 2-level sort on the raw data: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
15. Apply a 3-Color Scale on PO Amount in the raw data (Day 4)
16. Use =SUMIFS(H2:H221,E2:E221,"North",I2:I221,"Delayed") and compare it against what the Pivot Table shows for the same filter (Day 8)
17. Use =RIGHT(A2,4) to extract the PO number from PO ID in a helper column (Day 10)



ANSWERS : 


<img width="1526" height="792" alt="Screenshot 2026-08-28 133708" src="https://github.com/user-attachments/assets/bb8aaf8d-87f5-4320-b3af-9c19eb336b0d" />


<img width="1517" height="725" alt="Screenshot 2026-08-28 133819" src="https://github.com/user-attachments/assets/d4a659b7-756a-444a-a0c9-2fd33eae75af" />


<img width="1503" height="777" alt="Screenshot 2026-08-28 133849" src="https://github.com/user-attachments/assets/24701fd5-f19b-4e1f-b330-d41d2b0558ec" />


<img width="1532" height="726" alt="Screenshot 2026-08-28 133951" src="https://github.com/user-attachments/assets/5afb877a-cf64-4345-8368-89155990b883" />


<img width="4812" height="529" alt="Picture 5" src="https://github.com/user-attachments/assets/4446a01a-731e-4c5a-bf12-f217e64af89e" />


<img width="1527" height="695" alt="Screenshot 2026-08-28 135107" src="https://github.com/user-attachments/assets/9e940b07-638c-4b1d-a1f2-05ec86c1ddfe" />


<img width="1258" height="602" alt="Screenshot 2026-08-28 135202" src="https://github.com/user-attachments/assets/39bdf1a3-3165-41c0-bbbf-86cc682f05c7" />


<img width="1171" height="710" alt="Screenshot 2026-08-28 135255" src="https://github.com/user-attachments/assets/622e6913-968d-41c8-a902-c84f1d7cde54" />
