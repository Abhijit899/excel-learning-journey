Hard Q1 — SAP Vendor Master Text Cleaning 80 rows
This is a raw Vendor Master export from SAP — names in ALL CAPS, combined columns, extra spaces. Clean it using text formulas:

Add these columns:
Col H — Clean Vendor Name: =PROPER(TRIM(B2))
Col I — Vendor Name Length: =LEN(TRIM(B2))
Col J — First Word of Name: =LEFT(TRIM(B2),FIND(" ",TRIM(B2))-1)
Col K — Vendor Code from ID: =RIGHT(C2,3) — last 3 digits of Vendor ID
Col L — City extracted: =LEFT(D2,FIND(",",D2)-1) — City from "City, State"
Col M — State extracted: =TRIM(MID(D2,FIND(",",D2)+1,LEN(D2)))
Col N — Full Label: =PROPER(TRIM(B2))&" | "&E2&" | "&F2
Col O — Phone cleaned: =SUBSTITUTE(SUBSTITUTE(G2,"-","")," ","")
Col P — Category UPPER: =UPPER(F2)

Summary below data:
— Longest vendor name: =MAX(I2:I81)
— Shortest vendor name: =MIN(I2:I81)
— Count vendors from Maharashtra: =COUNTIF(M2:M81,"Maharashtra")

Revision tasks:
— Sort by Clean Vendor Name A to Z (revision)
— Filter State = Maharashtra (revision)
— CF: Category = "MACHINERY" → Blue fill on Category UPPER column (revision)


ANSWER :



Add these columns:
Col H — Clean Vendor Name: =PROPER(TRIM(B2))
Col I — Vendor Name Length: =LEN(TRIM(B2))
Col J — First Word of Name: =LEFT(TRIM(B2),FIND(" ",TRIM(B2))-1)
Col K — Vendor Code from ID: =RIGHT(C2,3) — last 3 digits of Vendor ID
Col L — City extracted: =LEFT(D2,FIND(",",D2)-1) — City from "City, State"
Col M — State extracted: =TRIM(MID(D2,FIND(",",D2)+1,LEN(D2)))
Col N — Full Label: =PROPER(TRIM(B2))&" | "&E2&" | "&F2
Col O — Phone cleaned: =SUBSTITUTE(SUBSTITUTE(G2,"-","")," ","")
Col P — Category UPPER: =UPPER(F2)


ANS . 


<img width="3088" height="1925" alt="Picture 28" src="https://github.com/user-attachments/assets/ba5977a2-e58e-4926-aa58-ed5cc4675b00" />


Summary below data:
— Longest vendor name: =MAX(I2:I81)
— Shortest vendor name: =MIN(I2:I81)
— Count vendors from Maharashtra: =COUNTIF(M2:M81,"Maharashtra")

ANS .


<img width="3155" height="2067" alt="Picture 29" src="https://github.com/user-attachments/assets/81cdbe1e-9fab-429b-8cf2-4375b8be67a0" />


Revision tasks:
— Sort by Clean Vendor Name A to Z (revision)
— Filter State = Maharashtra (revision)
— CF: Category = "MACHINERY" → Blue fill on Category UPPER column (revision)

ANS . 

— Sort by Clean Vendor Name A to Z (revision)


<img width="3155" height="1925" alt="Picture 31" src="https://github.com/user-attachments/assets/e204a067-22b2-4d85-9a4f-1b988875843d" />



— Filter State = Maharashtra (revision)


<img width="3155" height="406" alt="Picture 32" src="https://github.com/user-attachments/assets/ea28df2d-3cb3-47bf-8491-9709ed61351d" />



— CF: Category = "MACHINERY" → Blue fill on Category UPPER column (revision)


<img width="3155" height="1925" alt="Picture 33" src="https://github.com/user-attachments/assets/ad8b5abb-77c0-44c0-bc67-7e4343ef312b" />



---


Hard Q2 — SAP PO ID Text Extraction + Combining 80 rows
This SAP PO data has IDs and descriptions that need to be split, cleaned, and recombined:

Add these columns:
Col K — PO Prefix: =LEFT(A2,FIND("-",A2)-1) — extract "PO" from "PO-MM-1001"
Col L — PO Number: =RIGHT(A2,4) — last 4 digits
Col M — Vendor First Name: =LEFT(TRIM(D2),FIND(" ",TRIM(D2))-1)
Col N — Vendor Clean: =PROPER(TRIM(D2))
Col O — PO Label: =A2&" | "&PROPER(TRIM(D2))&" | "&TEXT(I2,"₹#,##0")
Col Q — Category Short: =LEFT(H2,3) — first 3 letters of category
Col R — Region Upper: =UPPER(E2)
Col S — Amount as Text: =TEXT(I2,"₹#,##0.00")
Col T — PO Month: =TEXT(B2,"MMM-YYYY") — format date as "Jan-2026"

Summary below data:
— Count POs with "North" in Region: =COUNTIF(E2:E81,"North")
— Total PO Amount: =SUM(I2:I81) (revision)
— Average PO Amount: =AVERAGE(I2:I81) (revision)
— 2nd Highest PO: =LARGE(I2:I81,2) (revision)

Revision tasks:
— CF: Delivery=Delayed → Orange row (revision)
— Sort: Region A to Z then PO Amount largest to smallest (revision)
— Convert to table named "POTextTable" (revision)


ANSWER : 



Add these columns:
Col K — PO Prefix: =LEFT(A2,FIND("-",A2)-1) — extract "PO" from "PO-MM-1001"
Col L — PO Number: =RIGHT(A2,4) — last 4 digits
Col M — Vendor First Name: =LEFT(TRIM(D2),FIND(" ",TRIM(D2))-1)
Col N — Vendor Clean: =PROPER(TRIM(D2))
Col O — PO Label: =A2&" | "&PROPER(TRIM(D2))&" | "&TEXT(I2,"₹#,##0")
Col Q — Category Short: =LEFT(H2,3) — first 3 letters of category
Col R — Region Upper: =UPPER(E2)
Col S — Amount as Text: =TEXT(I2,"₹#,##0.00")
Col T — PO Month: =TEXT(B2,"MMM-YYYY") — format date as "Jan-2026"

ANS .


<img width="4125" height="1925" alt="Picture 34" src="https://github.com/user-attachments/assets/cb84bf08-9c20-4540-9378-33846e49d9c7" />


Summary below data:
— Count POs with "North" in Region: =COUNTIF(E2:E81,"North")
— Total PO Amount: =SUM(I2:I81) (revision)
— Average PO Amount: =AVERAGE(I2:I81) (revision)
— 2nd Highest PO: =LARGE(I2:I81,2) (revision)


ANS .


<img width="4125" height="1925" alt="Picture 34" src="https://github.com/user-attachments/assets/4a241617-7e5d-4a34-a0c7-fb41473eb174" />


Revision tasks:
— CF: Delivery=Delayed → Orange row (revision)
— Sort: Region A to Z then PO Amount largest to smallest (revision)
— Convert to table named "POTextTable" (revision)


ANS .



<img width="1878" height="928" alt="Screenshot 2026-07-21 203504" src="https://github.com/user-attachments/assets/7083021f-b6be-4208-b487-939050b52287" />




<img width="4125" height="1925" alt="Picture 34" src="https://github.com/user-attachments/assets/ead10f87-dd53-4e76-b259-ff6fb7cea419" />

