Mini Project — SAP PO 3-Tier Risk & Attention Report 250 rows
Scenario: Your manager at Mahindra wants every PO automatically sorted into a risk tier using nested logic, AND flagged separately if it needs attention for any of several possible reasons. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "PO Risk & Attention" (double-click tab)
2. In column J, use =IF(OR(I2="Delayed",I2="Pending"),"Needs Attention","On Track")
3. In column K, use =IF(H2<50000,"Low",IF(H2<=200000,"Medium","High")) for a 3-tier amount classification
4. In column L, use =IF(OR(F2="North",F2="East"),"Priority Zone","Standard Zone") — OR on region
5. In column M, combine it all: =IF(AND(K2="High",J2="Needs Attention"),"🔴 Critical",IF(OR(K2="High",J2="Needs Attention"),"🟡 Watch","🟢 OK"))
6. Apply Conditional Formatting: Text Contains "Critical" on column M → Red Fill; "Watch" → Yellow Fill; "OK" → Green Fill
7. Turn on AutoFilter and filter column M to show only "🔴 Critical" rows — note how many need urgent attention
8. Clear the filter, sort by column K (using a Custom List: High, Medium, Low) so riskiest POs group at the top
9. Add a Summary block starting P1: P1="Total Rows", Q1=250; P2="Critical POs", Q2=count you observed; P3="Needs Attention", Q3=count you observed; P4="High Tier POs", Q4=count you observed
10. Save using Ctrl+S, then Save As (F12) → name it: new-day-07-if-or-nestedif-mahindra-po.xlsx
11. Create Sheet2 → rename "IF+OR & Nested IF Log" → write down every formula used today
12. Bold and underline the header row (Day 1)
13. Select PO Amount → Ctrl+Shift+$ Currency format (Day 1)
14. Select Qty column → Data Validation → Allow Whole Number → Between 1 and 100 (Day 3)
15. Apply Data Bars on Qty column (Day 4)
16. Run Data → Remove Duplicates on PO ID if any exist, confirm none were found (Day 5)



ANSWER : 



<img width="1558" height="6278" alt="Picture 2" src="https://github.com/user-attachments/assets/6772b50f-27bd-4dab-9b5d-be38c45d2d5c" />



<img width="1890" height="875" alt="Screenshot 2026-08-24 211426" src="https://github.com/user-attachments/assets/1f4d7df9-ada6-4987-9c7c-d67d71d4abf0" />
