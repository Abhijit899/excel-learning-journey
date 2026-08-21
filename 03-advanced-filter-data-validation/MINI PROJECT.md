Mini Project — SAP Clean Intake Sheet with Vendor Extraction 250 rows
Scenario: Your manager at Mahindra wants a fresh intake sheet where data entry mistakes are impossible going forward, PLUS a quick extracted list of every high-priority PO (North region OR high value) for tomorrow's review. Complete all tasks:

1. Paste data in Sheet1 → rename sheet to "Clean Intake Setup" (double-click tab)
2. Set up a Criteria Range for: Region="North" OR PO Amount>200000 (2 separate rows, matching column headers copied above)
3. Run Advanced Filter with that criteria, Copy to a new area starting at L1
4. Separately, extract a Unique list of all Category values into a new area using "Unique records only"
5. Apply Data Validation on Delivery Status column: Allow List → Delivered,Pending,Delayed
6. Apply Data Validation on Region column: Allow List → North,South,East,West
7. Apply Data Validation on Qty column: Allow Whole Number → Between 1 and 100, with an Input Message explaining the rule
8. Apply Data Validation on PO Amount column: Allow Custom → Formula ensuring value is greater than 0, with a clear Error Alert message
9. Use Circle Invalid Data to check the whole sheet for any rule violations already present
10. Add a Summary block starting from cell P1: P1="High-Priority POs Extracted", Q1=count you observed; P2="Unique Categories Found", Q2=count you observed; P3="Validation Rules Applied", Q3=4
11. Save using Ctrl+S, then Save As (F12) → name it: new-day-03-advfilter-datavalidation-mahindra-po.xlsx
12. Create Sheet2 → rename "Filter & Validation Log" → write down every criteria range and validation rule used today
13. Select PO Amount → Ctrl+Shift+$ Currency format (Day 1)
14. Bold and underline the header row using Ctrl+B then Ctrl+U (Day 1)
15. Data → Sort → 2-level sort: Region (A-Z) then PO Amount (Largest to Smallest) (Day 2)
16. Turn on AutoFilter, apply a Text Filter (Contains "Steel") on Vendor Name, then clear it (Day 2)


ANSWER :


<img width="6069" height="6027" alt="Picture 23" src="https://github.com/user-attachments/assets/7e9fa2c1-5b28-41c7-949f-ee19fc8408d6" />


<img width="2369" height="6027" alt="Picture 24" src="https://github.com/user-attachments/assets/3bf28037-0909-4e55-9ba9-be000f27ab68" />


<img width="3409" height="6027" alt="Picture 25" src="https://github.com/user-attachments/assets/a9659f89-5abf-449c-89a6-9af5cb5a5ee4" />


<img width="1138" height="6027" alt="Picture 26" src="https://github.com/user-attachments/assets/c614e5d3-987c-48c3-b809-0540b9099741" />


<img width="1273" height="706" alt="Screenshot 2026-08-21 170759" src="https://github.com/user-attachments/assets/17dca5c1-4f91-4b9f-920b-b152e480686f" />


<img width="1732" height="907" alt="Screenshot 2026-08-21 170606" src="https://github.com/user-attachments/assets/ef04ea0f-e0ed-4787-a702-aa78b3b9c3a2" />


<img width="1804" height="899" alt="Screenshot 2026-08-21 170537" src="https://github.com/user-attachments/assets/5c06b639-a6bb-4b44-976f-cddab5b91a23" />


<img width="1919" height="953" alt="Screenshot 2026-08-21 170421" src="https://github.com/user-attachments/assets/6186231b-3a3d-472d-bf34-ab448d1ce515" />


<img width="1834" height="972" alt="Screenshot 2026-08-21 154658" src="https://github.com/user-attachments/assets/327c88d7-3a9b-4523-9264-eccbfc48e5a4" />


<img width="1892" height="1009" alt="Screenshot 2026-08-21 154651" src="https://github.com/user-attachments/assets/f4f77fcb-eb9a-4666-a9a1-004335685668" />
