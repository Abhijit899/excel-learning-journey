Hard Q1 — SAP PO Regional Analysis 80 rows
Build a Summary Table below your data (row 85 onwards) using SUMIF, COUNTIF, AVERAGEIF:

Region-wise Summary (rows 85–90):
For each region — North, South, East, West:
— Total PO Amount: =SUMIF($E$2:$E$81,"North",$I$2:$I$81)
— Count of POs: =COUNTIF($E$2:$E$81,"North")
— Average PO Amount: =AVERAGEIF($E$2:$E$81,"North",$I$2:$I$81)

Delivery Status Summary (rows 92–95):
For Delivered, Pending, Delayed:
— Total PO Amount: SUMIF on Delivery Status
— Count: COUNTIF on Delivery Status
— Average: AVERAGEIF on Delivery Status

Payment Status Summary (rows 97–100):
For Paid, Pending, Overdue:
— Total: SUMIF | Count: COUNTIF | Average: AVERAGEIF

Amount-based Analysis (rows 102–106):
— Total POs above 3 lakhs: =SUMIF(I2:I81,">300000",I2:I81)
— Count POs above 3 lakhs: =COUNTIF(I2:I81,">300000")
— Total POs below 1 lakh: =SUMIF(I2:I81,"<100000",I2:I81)
— Count not Paid: =COUNTIF(K2:K81,"<>Paid")
— Average for vendors rated 4 or 5: =AVERAGEIF(H2:H81,">=4",I2:I81)

Vendor-wise (rows 108–112):
— Total spend on Tata Steel: =SUMIF(D2:D81,"Tata Steel",I2:I81)
— Count Tata Steel POs: =COUNTIF(D2:D81,"Tata Steel")
— Total spend on vendors with "Industries" in name: =SUMIF(D2:D81,"*Industries*",I2:I81)

Revision: CF Delayed=Orange | Sort by PO Amount largest first | Table named "POAnalysis"



ANSWER :


Region-wise Summary (rows 85–90):
For each region — North, South, East, West:
— Total PO Amount: =SUMIF($E$2:$E$81,"North",$I$2:$I$81)
— Count of POs: =COUNTIF($E$2:$E$81,"North")
— Average PO Amount: =AVERAGEIF($E$2:$E$81,"North",$I$2:$I$81)

Delivery Status Summary (rows 92–95):
For Delivered, Pending, Delayed:
— Total PO Amount: SUMIF on Delivery Status
— Count: COUNTIF on Delivery Status
— Average: AVERAGEIF on Delivery Status

Payment Status Summary (rows 97–100):
For Paid, Pending, Overdue:
— Total: SUMIF | Count: COUNTIF | Average: AVERAGEIF


ANS .


<img width="1408" height="2163" alt="Picture 49" src="https://github.com/user-attachments/assets/b72afad8-d196-49b0-8700-85ca298fc28b" />


Amount-based Analysis (rows 102–106):
— Total POs above 3 lakhs: =SUMIF(I2:I81,">300000",I2:I81)
— Count POs above 3 lakhs: =COUNTIF(I2:I81,">300000")
— Total POs below 1 lakh: =SUMIF(I2:I81,"<100000",I2:I81)
— Count not Paid: =COUNTIF(K2:K81,"<>Paid")
— Average for vendors rated 4 or 5: =AVERAGEIF(H2:H81,">=4",I2:I81)


ANS .

<img width="1519" height="2667" alt="Picture 50" src="https://github.com/user-attachments/assets/d2cdc7e8-3f53-466c-bc4a-9099d5abb0af" />



Vendor-wise (rows 108–112):
— Total spend on Tata Steel: =SUMIF(D2:D81,"Tata Steel",I2:I81)
— Count Tata Steel POs: =COUNTIF(D2:D81,"Tata Steel")
— Total spend on vendors with "Industries" in name: =SUMIF(D2:D81,"*Industries*",I2:I81)

Revision: CF Delayed=Orange | Sort by PO Amount largest first | Table named "POAnalysis"


Ans .


<img width="1871" height="950" alt="Screenshot 2026-07-26 200415" src="https://github.com/user-attachments/assets/c11d97ff-3065-49a2-8943-e69e42581c86" />



<img width="1746" height="2667" alt="Picture 52" src="https://github.com/user-attachments/assets/31a50dcb-b3dc-48f1-a242-41a7d1524e04" />


---


Hard Q2 — SAP Invoice Category Analysis 80 rows
Build a full summary using SUMIF, COUNTIF, AVERAGEIF:

Category-wise Summary:
For each category — Raw Material, Packaging, Machinery, Chemicals, IT Equipment, Office Supplies, Logistics, Utilities:
— Total Invoice Amount: SUMIF on Category
— Count of Invoices: COUNTIF on Category
— Average Invoice: AVERAGEIF on Category

State-wise Summary (top 5 states):
Maharashtra, Delhi, Karnataka, Tamil Nadu, Gujarat:
— Total: SUMIF | Count: COUNTIF | Average: AVERAGEIF

Additional Analysis:
— Total invoices above 4 lakhs: SUMIF
— Count invoices below 1 lakh: COUNTIF
— Count invoices NOT from Maharashtra: =COUNTIF(D2:D81,"<>Maharashtra")
— Average invoice for Paid status: AVERAGEIF
— Total for Overdue status: SUMIF
— Count vendors with "Ltd" in name: =COUNTIF(C2:C81,"*Ltd*")

Revision: CF Invoice above 5 lakhs=Red | Filter State=Maharashtra | Sort by Invoice Amount largest first



ANSWER : 


Category-wise Summary:
For each category — Raw Material, Packaging, Machinery, Chemicals, IT Equipment, Office Supplies, Logistics, Utilities:
— Total Invoice Amount: SUMIF on Category
— Count of Invoices: COUNTIF on Category
— Average Invoice: AVERAGEIF on Category


ANS .


