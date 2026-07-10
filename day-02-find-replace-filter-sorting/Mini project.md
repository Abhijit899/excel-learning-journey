Mini Project — SAP Procurement Cleaning & Priority Report 120 rows
Scenario: You are a junior SAP MM consultant at Bajaj Auto. You received a raw 120-row PO dump from SAP with errors, wrong status abbreviations, and missing values. Your manager needs a clean, sorted, filtered priority report by end of day.

Sheet 1 — "Raw Data": paste 120-row dataset as-is

Step 1 — Find & Replace (clean the data):
— Fix "Dlyd" → "Delayed" | "Pndg" → "Pending" | "Dlvd" → "Delivered"
— Fix "Ovrd" → "Overdue" | "Pd" → "Paid"
— Fix vendor typo: "Reliance Indstries" → "Reliance Industries"

Step 2 — Go To Special:
— Find all blank cells in PO Amount column → fill with 0 using Ctrl+Enter
— Find all blank cells in Delivery Status → fill with "Pending"

Step 3 — Formatting (revision from Day 1):
— Header: Bold, Dark Blue background, White font
— PO Amount: Accounting format ₹
— Add Sr No column using Fill Series
— Add GST column: =PO Amount × 18%
— Add Total with GST column

Step 4 — Conditional Formatting (revision):
— Delayed = Orange row | Pending = Yellow row | Delivered = Green row
— Overdue = Red font | PO Amount above 3,00,000 = Bold Red font

Step 5 — Sorting:
— Multi-level: Payment Status (Overdue → Pending → Paid) then PO Amount (Largest → Smallest)

Step 6 — Filter & Copy:
— Filter to show only Delayed + Overdue rows
— Go To Special → Visible Cells Only → Copy
— Paste Special → Values + Formats into Sheet 2 named "Priority Report"

Step 7 — Clear:
— Clear all filters in Sheet 1
— Clear any stray formatting in empty columns


ANSWER :


Step 1 — Find & Replace (clean the data):
— Fix "Dlyd" → "Delayed" | "Pndg" → "Pending" | "Dlvd" → "Delivered"
— Fix "Ovrd" → "Overdue" | "Pd" → "Paid"
— Fix vendor typo: "Reliance Indstries" → "Reliance Industries"

Ans. 


<img width="1238" height="2905" alt="Picture 2" src="https://github.com/user-attachments/assets/ba0c8903-d16a-4644-88e1-73e7f0c85ab6" />


Step 2 — Go To Special:
— Find all blank cells in PO Amount column → fill with 0 using Ctrl+Enter
— Find all blank cells in Delivery Status → fill with "Pending"

Ans. 


<img width="1238" height="2905" alt="Picture 3" src="https://github.com/user-attachments/assets/5b91c76a-9a77-4b81-baf6-6afa0837c6f2" />


Step 3 — Formatting (revision from Day 1):
— Header: Bold, Dark Blue background, White font
— PO Amount: Accounting format ₹
— Add Sr No column using Fill Series
— Add GST column: =PO Amount × 18%
— Add Total with GST column


Ans. 


<img width="1318" height="2905" alt="Picture 4" src="https://github.com/user-attachments/assets/432187e1-7291-4e02-90d7-1255a2c1d49c" />


<img width="1546" height="2905" alt="Picture 5" src="https://github.com/user-attachments/assets/746c2321-2d87-459d-a7db-e7f597b521f7" />


Step 4 — Conditional Formatting (revision):
— Delayed = Orange row | Pending = Yellow row | Delivered = Green row
— Overdue = Red font | PO Amount above 3,00,000 = Bold Red font


Ans. 


<img width="1546" height="2905" alt="Picture 6" src="https://github.com/user-attachments/assets/5bfa741e-55a5-4992-b704-7a905048a436" />


Step 5 — Sorting:
— Multi-level: Payment Status (Overdue → Pending → Paid) then PO Amount (Largest → Smallest)

Ans. 


<img width="1546" height="2905" alt="Picture 7" src="https://github.com/user-attachments/assets/6005b147-1e08-42cc-8c2a-7bfa99c3da7d" />


Step 6 — Filter & Copy:
— Filter to show only Delayed + Overdue rows
— Go To Special → Visible Cells Only → Copy
— Paste Special → Values + Formats into Sheet 2 named "Priority Report"

Ans. 


