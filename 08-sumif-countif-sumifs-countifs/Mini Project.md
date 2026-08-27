Mini Project — SAP Regional & Category Spend Summary 250 rows
Scenario: Your manager at Mahindra wants a summary block showing total spend, count, and breakdown by Region and Category — without a Pivot Table yet. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "Regional Spend Summary" (double-click tab)
2. Build a small table starting L1 with 4 Regions listed down column L (North, South, East, West)
3. In M2:M5, use =SUMIF($F$2:$F$251,L2,$H$2:$H$251) fill down — total PO Amount per Region
4. In N2:N5, use =COUNTIF($F$2:$F$251,L2) fill down — count of POs per Region
5. Build a second table starting Q1 listing all 8 Categories down column Q
6. In R2:R9, use =SUMIFS($H$2:$H$251,$G$2:$G$251,Q2,$I$2:$I$251,"Delayed") — total Delayed PO Amount per Category
7. In S2:S9, use =COUNTIFS($G$2:$G$251,Q2,$I$2:$I$251,"Delayed") — count of Delayed POs per Category
8. Apply Data Bars on columns M and R for visual comparison
9. Add a Summary block starting V1: V1="Highest Spend Region", W1=region you observed; V2="Highest Delayed-Spend Category", W2=category you observed; V3="Total Rows", W3=250
10. Save using Ctrl+S, then Save As (F12) → name it: new-day-08-sumif-countif-sumifs-countifs-mahindra-po.xlsx
11. Create Sheet2 → rename "Aggregation Formula Log" → write down every formula used today
12. Bold and underline the header row (Day 1)
13. Turn on AutoFilter, filter Delivery Status = "Delayed" then clear (Day 2)
14. Select PO Amount → Data Validation → Allow Custom → Formula ensuring value greater than 0 (Day 3)
15. Use Flash Fill (Ctrl+E) if useful on any text column (Day 4)
16. Run Data → Remove Duplicates on PO ID, confirm none found (Day 5)
17. Use =IF(H2<50000,"Low",IF(H2<=200000,"Medium","High")) as a nested IF tier column (Day 7)



ANSWERS : 


<img width="1841" height="6278" alt="Picture 5" src="https://github.com/user-attachments/assets/de13619a-1d35-4b3d-8945-b3a2325dc07b" />



<img width="1841" height="1903" alt="Picture 6" src="https://github.com/user-attachments/assets/44165d36-689c-400a-967b-9e56b1412387" />



<img width="1946" height="6278" alt="Picture 7" src="https://github.com/user-attachments/assets/ff2cc349-59ec-439c-ae9d-e03272355502" />
