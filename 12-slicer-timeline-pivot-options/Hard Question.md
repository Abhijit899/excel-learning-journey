Business Question Answer in 1 line
A SAP MM consultant wants their manager to click simple buttons to filter a Pivot Table by Region or Category during a live review, AND wants a slider to filter by month instead of digging through a date dropdown. Which two features achieve this, one for each need?



ANSWER : 






---



Hard Question — Full Slicer & Timeline Drill 220 rows · single combined question
Paste this data in Sheet1. Convert it to a Table (Ctrl+T) first. Complete every task below in order:

1. Select any cell in the Table → Insert → PivotTable → New Worksheet → OK
2. Build the Pivot Table: Region in Rows, PO Amount in Values (Sum), Category in Values (Count)
3. Click inside the Pivot Table → Insert → Slicer → tick Region and Category → OK — confirm two slicer boxes appear
4. Click "North" on the Region slicer — confirm the Pivot Table filters instantly
5. Hold Ctrl and click "South" as well on the same slicer — confirm BOTH North and South now show together
6. Click the funnel-with-X icon on the Region slicer to clear that filter
7. Go back to your raw data sheet → build a 2nd small Pivot Table (Insert → PivotTable → Existing Worksheet, place it a few columns away) with Category in Rows and PO Amount in Values
8. Right-click your Region slicer → Report Connections → tick the 2nd Pivot Table too — confirm clicking the slicer now filters BOTH tables at once
9. Click inside the first Pivot Table → Insert → Timeline → choose Order Date → OK
10. Click the timeline's month view and drag to select just 2-3 months — confirm the Pivot Table filters to that period
11. Right-click the Pivot Table → PivotTable Options → Totals & Filters tab → untick "Show grand totals for rows" → OK — confirm the grand total row disappears
12. On the Design tab, change Report Layout to "Show in Tabular Form" — observe how the layout changes from Compact to Tabular
13. Use the Name Box to jump directly to K1 on your raw data sheet, then Ctrl+Home back to A1 (Day 1)
14. Data → Sort → 2-level sort on raw data: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
15. Apply a 3-Color Scale on PO Amount in raw data (Day 4)
16. Use =SUMIFS(H2:H221,E2:E221,"North",I2:I221,"Delayed") and compare against the slicer-filtered Pivot Table total (Day 8)
17. Insert a PivotChart (Column) from your first Pivot Table and confirm it also responds to the slicer (Day 11)


ANSWERS : 



<img width="1421" height="606" alt="Screenshot 2026-08-28 160307" src="https://github.com/user-attachments/assets/4340d4b5-daac-49a1-9dca-b529d3b25422" />


<img width="1465" height="533" alt="Screenshot 2026-08-28 160331" src="https://github.com/user-attachments/assets/f38377db-c1e5-4178-bdcd-3c079061babb" />


<img width="1457" height="458" alt="Screenshot 2026-08-28 160404" src="https://github.com/user-attachments/assets/1ae48cf8-7069-4622-bdf7-27aeefaca0df" />


<img width="1532" height="603" alt="Screenshot 2026-08-28 160629" src="https://github.com/user-attachments/assets/3bf71496-87c2-4bfe-b9a7-2e14d6048e5a" />


<img width="1043" height="533" alt="Screenshot 2026-08-28 160712" src="https://github.com/user-attachments/assets/e8184d88-a7bb-46bd-b25d-f43592285139" />


<img width="1522" height="565" alt="Screenshot 2026-08-28 160801" src="https://github.com/user-attachments/assets/f52b0f78-9547-4d6b-b260-302aaa544e49" />


<img width="1503" height="607" alt="Screenshot 2026-08-28 160959" src="https://github.com/user-attachments/assets/ebcd957b-51d1-48a2-ab13-9394a5c66e3b" />


