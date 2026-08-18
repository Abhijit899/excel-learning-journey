<img width="1138" height="2091" alt="Picture 11" src="https://github.com/user-attachments/assets/6426da00-8bb7-4ef1-a164-d4f934230265" />Business Question 

A SAP MM consultant needs a report sorted first by Region (A to Z), then by PO Amount (highest to lowest) WITHIN each region — and after that, wants to see only the rows where Delivery Status is "Delayed".
Which two Excel features, used one after the other, achieve both steps?


ANSWER : 

Sort → Filter



---


Hard Question — Full Sort & Filter Drill 220 rows · single combined question
Paste this data. Complete every task below in order:

1. Select any PO Amount cell → Data → Sort Largest to Smallest → when the Sort Warning appears, choose "Expand the selection"
2. Undo (Ctrl+Z), then repeat but choose "Continue with the current selection" instead — observe how Vendor Names no longer match their correct PO IDs, then Undo again
3. Open Data → Sort → set Level 1 = Region (A to Z), Level 2 = PO Amount (Largest to Smallest)
4. Add a 3rd sort level: Delivery Status (A to Z)
5. Turn on AutoFilter using Ctrl+Shift+L
6. Filter Delivery Status to show only "Delayed"
7. Also filter Region to only "North" at the same time — confirm both filters apply together
8. Note how many rows remain visible after both filters
9. Clear all filters using Alt, A, C
10. Click the Vendor Name dropdown → Text Filters → Contains → type "Steel" → OK — confirm only Steel vendors show
11. Clear that filter → click PO Amount dropdown → Number Filters → Between → type 50000 and 150000 → OK
12. Clear that filter → apply a Number Filter on PO Amount → Top 10 Items — note which 2-3 vendors dominate
13. Clear filters again, then re-sort by PO ID (A to Z) to restore a clean original order before saving
14. Use the Name Box to jump directly to K1, then Ctrl+Home back to A1
15. Use =SUM(I2:I221) with Alt+= to confirm the total PO value
16. Select PO Amount → Ctrl+Shift+$ Currency format


ANSWER : 


<img width="1138" height="5307" alt="Picture 9" src="https://github.com/user-attachments/assets/6a72bae0-d7ec-4ab4-8255-90e6320325f8" />


<img width="1138" height="1611" alt="Picture 10" src="https://github.com/user-attachments/assets/9c0f28fe-8816-4214-b9d7-37caf9f1da73" />


<img width="1138" height="2091" alt="Picture 11" src="https://github.com/user-attachments/assets/93ca14a3-43e1-42aa-83d5-5fbc61b037b7" />


<img width="1138" height="5331" alt="Picture 12" src="https://github.com/user-attachments/assets/5c71b6fc-ec22-48e6-8d32-ccb7a2931de5" />


<img width="1824" height="898" alt="Screenshot 2026-08-18 205912" src="https://github.com/user-attachments/assets/77ba9b67-da7a-4057-8cbe-1c7e5354c743" />


<img width="1382" height="701" alt="Screenshot 2026-08-18 210521" src="https://github.com/user-attachments/assets/2fc4b727-0263-4a90-aa9d-1962c46c3c7c" />


<img width="1464" height="751" alt="Screenshot 2026-08-18 210908" src="https://github.com/user-attachments/assets/ae019cbd-1656-4c67-8c55-804cbd3e8d0a" />


<img width="1307" height="755" alt="Screenshot 2026-08-18 211104" src="https://github.com/user-attachments/assets/633b32ee-4882-401e-8c2d-d6864d8b7877" />
