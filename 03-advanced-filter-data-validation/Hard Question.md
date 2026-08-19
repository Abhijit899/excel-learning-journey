Business Question Answer in 1 line
A SAP MM consultant wants to (1) extract a list of PO rows where Region="North" OR Delivery Status="Delayed" into a separate area, and (2) stop anyone from typing free text into the Delivery Status column going forward, forcing them to pick from a fixed list instead.
Which two specific features from today solve each part?


ANSWER : 


Filter and Data Validation


---


Hard Question — Full Advanced Filter & Data Validation Drill 220 rows · single combined question
Paste this data. Complete every task below in order:

Advanced Filter:
1. In K1:S1, copy the header row. In K2, type "North" under the Region header — this is your Criteria Range for a single AND condition
2. Data → Advanced → List Range = A1:I221, Criteria Range = K1:S2, Copy to = U1 → run it, confirm only North rows appear at U1
3. Now add a 2nd criteria row: in K3, leave Region blank, but under Delivery Status (column matching in your criteria range) type "Delayed" — this makes it Region=North OR Delivery Status=Delayed
4. Re-run Advanced Filter with the updated criteria range (K1:S3), Copy to a new area → confirm more rows appear than step 2
5. Clear the criteria rows, set List Range to just the Vendor Name column, tick "Unique records only", Copy to another area → confirm you get exactly 25 unique vendor names
Data Validation:
6. Select the Delivery Status column (I2:I221) → Data → Data Validation → Allow: List → Source: Delivered,Pending,Delayed → OK — confirm a dropdown arrow appears
7. Try typing "Deliverd" (typo) directly into one cell in that column — confirm Excel blocks it with an error
8. Select the Qty column (H2:H221) → Data Validation → Allow: Whole Number → Between 1 and 100 → add an Input Message: "Enter quantity 1-100"
9. Select PO Amount column → Data Validation → Allow: Custom → Formula: =I2>0 → add an Error Alert titled "Invalid Amount" with message "PO Amount must be greater than 0"
10. Manually type -500 into one PO Amount cell to confirm the Custom validation blocks it, then undo
11. Use Data → Data Validation dropdown → Circle Invalid Data → check if any existing cells in the sheet violate your new rules
12. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1 (Day 1)
13. Use =SUM(I2:I221) with Alt+= to confirm the total PO value (Day 1)
14. Sort by Region (A-Z) then PO Amount (Largest to Smallest) — 2-level sort (Day 2)
15. Turn on AutoFilter (Ctrl+Shift+L), filter Delivery Status = "Delayed" only, then clear filters (Day 2)


ANSWER : 


<img width="3340" height="5307" alt="Picture 17" src="https://github.com/user-attachments/assets/04c32682-b38a-4b92-8f5c-a83c1497fb37" />


<img width="3340" height="5307" alt="Picture 18" src="https://github.com/user-attachments/assets/41edba93-668e-4f8c-8756-855ceca06ea6" />


<img width="3340" height="2403" alt="Picture 19" src="https://github.com/user-attachments/assets/f1a3701e-bfa9-42d1-8f48-51a8121c1fa2" />


<img width="3486" height="2403" alt="Picture 20" src="https://github.com/user-attachments/assets/a2bef69b-f4b3-4427-9e23-5d2a3ec40b09" />


<img width="1835" height="813" alt="Screenshot 2026-08-19 204325" src="https://github.com/user-attachments/assets/e24e016c-c5fa-4952-90c9-f5946a1dbb5f" />


<img width="1916" height="847" alt="Screenshot 2026-08-19 203902" src="https://github.com/user-attachments/assets/93d3e8c5-b759-46dc-948d-7c62c7b2be9d" />


<img width="1903" height="906" alt="Screenshot 2026-08-19 203519" src="https://github.com/user-attachments/assets/a6f57696-03d4-4fe3-a6ad-a8bc1c4b681b" />


<img width="453" height="221" alt="Screenshot 2026-08-19 203509" src="https://github.com/user-attachments/assets/c500534c-7937-40fa-8ff9-80d50411409d" />


<img width="1091" height="5355" alt="Picture 21" src="https://github.com/user-attachments/assets/bd6f45f6-c059-4e26-8f22-bdbdc2a23be4" />


<img width="1091" height="1633" alt="Picture 22" src="https://github.com/user-attachments/assets/401a83dc-31eb-4842-a90e-07b3d6b5e66c" />
