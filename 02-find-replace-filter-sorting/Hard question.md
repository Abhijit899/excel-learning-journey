Hard Q1 — SAP PO Data Cleaning & Filtering 80 rows
This is a raw PO export from SAP with errors and messy data. Complete all tasks:

Find & Replace Tasks:
1. Find "Dlyd" → Replace with "Delayed" (fixing abbreviation error in Delivery Status)
2. Find "Pndg" → Replace with "Pending"
3. Find "Dlvd" → Replace with "Delivered"
4. Find "Tata Steeel" → Replace with "Tata Steel" (fixing typo in vendor name)
5. Find all blank cells in PO Amount column (Ctrl+G → Special → Blanks) → type 0 → Ctrl+Enter

Go To Special Tasks:
6. Select all formula cells in sheet — how many formula cells are there? Write answer below data.
7. After applying filter (step below) — use Go To Special → Visible Cells Only before copying filtered data

Clear Tasks:
8. Select columns M onwards (empty columns) → Clear All to remove any stray formatting

Filter Tasks:
9. Filter Delivery Status = Delayed only — how many rows show? Write answer below data.
10. Clear filter. Filter Payment Status = Overdue only — how many rows?
11. Filter Region = North AND Delivery Status = Delayed together — how many rows?
12. Filter PO Amount greater than 3,00,000 — how many rows?
13. Clear filter. Apply Color filter — first apply CF (Delayed=Orange), then filter by Orange color

Paste Special Task:
14. Copy PO Amount column → Paste Special → Values Only into a new column — to remove any formulas
15. In a blank cell type 1.18 → Copy it → Select all PO Amount values → Paste Special → Multiply → this applies 18% GST in one step. Undo after confirming it works.


ANSWERS :



Find & Replace Tasks:
1. Find "Dlyd" → Replace with "Delayed" (fixing abbreviation error in Delivery Status)
2. Find "Pndg" → Replace with "Pending"
3. Find "Dlvd" → Replace with "Delivered"
4. Find "Tata Steeel" → Replace with "Tata Steel" (fixing typo in vendor name)
5. Find all blank cells in PO Amount column (Ctrl+G → Special → Blanks) → type 0 → Ctrl+Enter

Ans. 

<img width="1156" height="1944" alt="Picture 15" src="https://github.com/user-attachments/assets/a66bf73b-88aa-4886-806d-b457339c7e87" />


Go To Special Tasks:
6. Select all formula cells in sheet — how many formula cells are there? Write answer below data.
7. After applying filter (step below) — use Go To Special → Visible Cells Only before copying filtered data

Ans. 


6. No cells are found

   
7. <img width="1395" height="779" alt="Screenshot 2026-07-10 103802" src="https://github.com/user-attachments/assets/73fe78f0-2388-417d-99f9-aa93db0039af" />



Filter Tasks:
9. Filter Delivery Status = Delayed only — how many rows show? Write answer below data.
10. Clear filter. Filter Payment Status = Overdue only — how many rows?
11. Filter Region = North AND Delivery Status = Delayed together — how many rows?
12. Filter PO Amount greater than 3,00,000 — how many rows?
13. Clear filter. Apply Color filter — first apply CF (Delayed=Orange), then filter by Orange color


Ans.



<img width="1528" height="329" alt="Screenshot 2026-07-10 102432" src="https://github.com/user-attachments/assets/83936c74-533c-46c9-8ab3-475968120d5c" />


<img width="1173" height="672" alt="Screenshot 2026-07-10 103351" src="https://github.com/user-attachments/assets/134ec71f-032e-436c-9a8c-c4e848db4d65" />



Paste Special Task:
14. Copy PO Amount column → Paste Special → Values Only into a new column — to remove any formulas
15. In a blank cell type 1.18 → Copy it → Select all PO Amount values → Paste Special → Multiply → this applies 18% GST in one step. Undo after confirming it works.


Ans.



<img width="1348" height="1945" alt="Picture 17" src="https://github.com/user-attachments/assets/114c7f8d-9f79-4c53-8dbf-a83a2e926db5" />



---



Hard Q2 — SAP Invoice Sorting & Analysis 80 rows
This is a Vendor Invoice Register. Complete all sorting and filter tasks:

Sorting Tasks:
1. Add Sr No column (1–80) first before any sorting
2. Single sort: Invoice Amount — Largest to Smallest
3. Undo. Single sort: Vendor Name — A to Z
4. Undo. Multi-level sort: Region (A→Z) then Invoice Amount (Largest to Smallest)
5. Undo. Multi-level sort: Payment Status Custom Order (Overdue → Pending → Paid) then Invoice Amount (Largest to Smallest)
6. Undo. Sort by Cell Color — first apply CF (Overdue=Red, Pending=Yellow, Paid=Green) then sort Red on top, Yellow next, Green last

Filter Tasks:
7. Filter State = Maharashtra — how many invoices?
8. Filter Invoice Amount between 1,00,000 and 3,00,000
9. Filter Vendor Name contains "Tata" — how many rows?
10. Filter Payment Status = Overdue AND Region = South together
11. Filter Invoice Date — This Quarter option (Q2 2026)
12. Clear all filters. Apply Number Filter on Invoice Amount → Top 10 — what are the top 10 amounts?

Paste Special Task:
13. Copy the entire formatted report → Paste Special → Values + Formats into a new sheet called "Final Report" — this is how you share a clean copy without formulas


ANSWERS :



Sorting Tasks:
1. Add Sr No column (1–80) first before any sorting
2. Single sort: Invoice Amount — Largest to Smallest
3. Undo. Single sort: Vendor Name — A to Z
4. Undo. Multi-level sort: Region (A→Z) then Invoice Amount (Largest to Smallest)
5. Undo. Multi-level sort: Payment Status Custom Order (Overdue → Pending → Paid) then Invoice Amount (Largest to Smallest)
6. Undo. Sort by Cell Color — first apply CF (Overdue=Red, Pending=Yellow, Paid=Green) then sort Red on top, Yellow next, Green last

Ans .


1. <img width="1135" height="1947" alt="Picture 18" src="https://github.com/user-attachments/assets/911f49a5-2a85-4628-84ef-0eb79c29d323" />

2.<img width="1135" height="1947" alt="Picture 18" src="https://github.com/user-attachments/assets/dc13a58c-f78e-45f7-8f46-8da2cf9b49c2" />

3. <img width="1135" height="1947" alt="Picture 19" src="https://github.com/user-attachments/assets/02458c48-af3f-4474-9460-e7e1f958d401" />

4. <img width="1135" height="1947" alt="Picture 20" src="https://github.com/user-attachments/assets/630d42d4-902b-4deb-beb7-5310acf3ce5a" />

5. <img width="1114" height="1947" alt="Picture 21" src="https://github.com/user-attachments/assets/6602ea46-0dc9-4a47-ae43-81a9e49437c8" />

6. <img width="1135" height="1971" alt="Picture 22" src="https://github.com/user-attachments/assets/fb0a8d3c-c600-4554-9259-02713371ba71" />




Filter Tasks:
7. Filter State = Maharashtra — how many invoices?
8. Filter Invoice Amount between 1,00,000 and 3,00,000
9. Filter Vendor Name contains "Tata" — how many rows?
10. Filter Payment Status = Overdue AND Region = South together
11. Filter Invoice Date — This Quarter option (Q2 2026)
12. Clear all filters. Apply Number Filter on Invoice Amount → Top 10 — what are the top 10 amounts?


Ans. 

7. <img width="1453" height="414" alt="Screenshot 2026-07-10 120204" src="https://github.com/user-attachments/assets/5241efd2-9518-449d-b7c3-1eb46a835f75" />


8.<img width="1135" height="915" alt="Picture 23" src="https://github.com/user-attachments/assets/1e0e3dc5-4853-4ec5-9453-19322e925233" />


9. <img width="1405" height="260" alt="Screenshot 2026-07-10 120833" src="https://github.com/user-attachments/assets/acc2e384-6e93-4fe3-8d8d-d9cf2ff52913" />


10. <img width="1272" height="221" alt="Screenshot 2026-07-10 120933" src="https://github.com/user-attachments/assets/d4e157bd-4684-4de8-82a7-7208ff54bd31" />


11. <img width="1439" height="699" alt="Screenshot 2026-07-10 121112" src="https://github.com/user-attachments/assets/c98586bb-48d6-4135-942b-b5f4d00c94a7" />


12. <img width="1322" height="368" alt="Screenshot 2026-07-10 121236" src="https://github.com/user-attachments/assets/890e6205-e455-4576-8572-aebe1df20a3d" />




Paste Special Task:
13. Copy the entire formatted report → Paste Special → Values + Formats into a new sheet called "Final Report" — this is how you share a clean copy without formulas


Ans. 


13.  <img width="1649" height="941" alt="Screenshot 2026-07-10 121736" src="https://github.com/user-attachments/assets/9e729244-8f2c-467f-9e4c-51ba5e66ac8b" />
