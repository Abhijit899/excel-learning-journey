Mini Project — SAP Monthly PO Dashboard Prep 120 rows
Scenario: You are a junior SAP MM consultant at Tata Motors. Every month end, you receive a raw PO dump from SAP. Before sending it to management, you must format it professionally and flag all issues visually.

Sheet 1 — "Raw PO Data": paste 120-row dataset

Step 1 — Data Entry & Fill Series:
— Add Sr No column (1–120) using Fill Series
— Add a "FY" column using Fill Series logic: type FY2026-27 and fill down

Step 2 — Formatting:
— Header row: Bold, Dark Blue background, White font, center aligned
— PO Amount column: Accounting format with ₹, 2 decimals
— Order Date: DD-MMM-YYYY format
— All number columns: right aligned
— Apply borders to entire table
— Wrap text in Vendor Name column
— Freeze top row

Step 3 — Number Calculations (new columns):
— GST 18%: =PO Amount × 18%
— Total with GST: =PO Amount + GST
— Format both as Accounting ₹

Step 4 — Conditional Formatting:
— Delivery Status = Delayed → Orange entire row
— Delivery Status = Pending → Yellow entire row
— Delivery Status = Delivered → Green entire row
— Payment Status = Overdue → Red font entire row
— PO Amount above 3,00,000 → Bold Red font
— Color Scale on PO Amount (Green=high, Red=low)
— Data Bars on Qty column
— Icon Set (3 traffic lights) on Vendor Rating column

Sheet 2 — "Summary":
— Manually type these labels and leave value cells blank for now (formulas come in next topics):
Total PO Amount | Average PO | Highest PO | Lowest PO | Count Delayed | Count Overdue



ANSWERS :

Sheet 1 — "Raw PO Data": paste 120-row dataset

Step 1 — Data Entry & Fill Series:
— Add Sr No column (1–120) using Fill Series
— Add a "FY" column using Fill Series logic: type FY2026-27 and fill down

Ans.

<img width="1591" height="2904" alt="Picture 13" src="https://github.com/user-attachments/assets/527beff7-8d4c-4a43-9c19-ca89969c3da6" />



Step 2 — Formatting:
— Header row: Bold, Dark Blue background, White font, center aligned
— PO Amount column: Accounting format with ₹, 2 decimals
— Order Date: DD-MMM-YYYY format
— All number columns: right aligned
— Apply borders to entire table
— Wrap text in Vendor Name column
— Freeze top row

Ans. 

<img width="1504" height="2904" alt="Picture 15" src="https://github.com/user-attachments/assets/942efde3-6cd1-42e1-9b09-a0d37232f21d" />


Step 3 — Number Calculations (new columns):
— GST 18%: =PO Amount × 18%
— Total with GST: =PO Amount + GST
— Format both as Accounting ₹

Ans. 


<img width="1732" height="2904" alt="Picture 15" src="https://github.com/user-attachments/assets/3ac6be24-ba24-45e6-abc5-3e6511de44f6" />


Step 4 — Conditional Formatting:
— Delivery Status = Delayed → Orange entire row
— Delivery Status = Pending → Yellow entire row
— Delivery Status = Delivered → Green entire row
— Payment Status = Overdue → Red font entire row
— PO Amount above 3,00,000 → Bold Red font
— Color Scale on PO Amount (Green=high, Red=low)
— Data Bars on Qty column
— Icon Set (3 traffic lights) on Vendor Rating column


Ans. 


<img width="1732" height="2904" alt="Picture 17" src="https://github.com/user-attachments/assets/52807220-911c-48f0-b151-c264191112c7" />


<img width="1732" height="2904" alt="Picture 16" src="https://github.com/user-attachments/assets/98046d15-d371-47c9-b949-df4e0615424a" />




Sheet 2 — "Summary":
— Manually type these labels and leave value cells blank for now (formulas come in next topics):
Total PO Amount | Average PO | Highest PO | Lowest PO | Count Delayed | Count Overdue


<img width="2142" height="2904" alt="Picture 19" src="https://github.com/user-attachments/assets/a254e1b7-cb38-48ef-9a4d-b5bcd03ee080" />
