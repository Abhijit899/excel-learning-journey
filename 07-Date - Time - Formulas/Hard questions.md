Hard Q1 — SAP PO Date Analysis 80 rows
Add these calculated columns:
Col K — Days Open: =TODAY()-B2 (format as Number)
Col L — Lead Time (days): =C2-B2
Col M — Working Days Lead Time: =NETWORKDAYS(B2,C2)
Col N — Payment Due Date: =EOMONTH(B2,1)
Col O — Contract Expiry (12 months): =EDATE(B2,12)
Col P — Expected Delivery (10 working days): =WORKDAY(B2,10)
Col Q — Order Month: =MONTH(B2)
Col R — Order Year: =YEAR(B2)
Col S — Week Number: =WEEKNUM(B2)
Col T — Overdue Flag: =IF((TODAY()-C2)>30,"Overdue","On Track")
Col U — Days Overdue: =IF(TODAY()-C2>0,TODAY()-C2,0)
Col V — Month Name: =TEXT(B2,"MMM-YYYY")

Summary below row 82:
— Average Lead Time: =AVERAGE(L2:L81)
— Max Lead Time: =MAX(L2:L81)
— Min Lead Time: =MIN(L2:L81)
— Count Overdue: =COUNTIF(T2:T81,"Overdue")
— Earliest Order: =MIN(B2:B81)
— Latest Order: =MAX(B2:B81)

Revision: CF Overdue=Orange row | Sort Days Overdue largest first


ANSWERS :



Add these calculated columns:
Col K — Days Open: =TODAY()-B2 (format as Number)
Col L — Lead Time (days): =C2-B2
Col M — Working Days Lead Time: =NETWORKDAYS(B2,C2)
Col N — Payment Due Date: =EOMONTH(B2,1)
Col O — Contract Expiry (12 months): =EDATE(B2,12)
Col P — Expected Delivery (10 working days): =WORKDAY(B2,10)
Col Q — Order Month: =MONTH(B2)
Col R — Order Year: =YEAR(B2)
Col S — Week Number: =WEEKNUM(B2)
Col T — Overdue Flag: =IF((TODAY()-C2)>30,"Overdue","On Track")
Col U — Days Overdue: =IF(TODAY()-C2>0,TODAY()-C2,0)
Col V — Month Name: =TEXT(B2,"MMM-YYYY")



ANS .


<img width="2937" height="1925" alt="Picture 41" src="https://github.com/user-attachments/assets/2991dbd2-fbc1-440b-9cb9-4d0f7f46dfb5" />



Summary below row 82:
— Average Lead Time: =AVERAGE(L2:L81)
— Max Lead Time: =MAX(L2:L81)
— Min Lead Time: =MIN(L2:L81)
— Count Overdue: =COUNTIF(T2:T81,"Overdue")
— Earliest Order: =MIN(B2:B81)
— Latest Order: =MAX(B2:B81)

Revision: CF Overdue=Orange row | Sort Days Overdue largest first


ANS .


<img width="2996" height="2067" alt="Picture 42" src="https://github.com/user-attachments/assets/a64f5616-5b6c-4a97-8c5f-f635395fa55d" />



---


Hard Q2 — SAP Vendor Contract Tracker 80 rows
Add these columns:
Col H — Contract Age (years): =DATEDIF(C2,TODAY(),"Y")
Col I — Contract Age (months): =DATEDIF(C2,TODAY(),"M")
Col J — Contract Age (days): =DATEDIF(C2,TODAY(),"D")
Col K — Expiry Date: =EDATE(C2,D2)
Col L — Days to Expiry: =K2-TODAY()
Col M — Status: =IF(K2<TODAY(),"EXPIRED","ACTIVE")
Col N — Days since Last Review: =TODAY()-E2
Col O — Next Review Due: =EDATE(E2,6)
Col P — Review Status: =IF(TODAY()>O2,"Review Overdue","OK")
Col Q — Expiry Month: =TEXT(K2,"MMM-YYYY")
Col R — Yearfrac: =ROUND(YEARFRAC(C2,TODAY()),1)

Summary below data:
— Count Active: =COUNTIF(M2:M81,"ACTIVE")
— Count Expired: =COUNTIF(M2:M81,"EXPIRED")
— Count Review Overdue: =COUNTIF(P2:P81,"Review Overdue")
— Average age months: =AVERAGE(I2:I81)

Revision: CF Expired=Red row | Days to Expiry below 90=Orange | Sort Days to Expiry smallest first



ANSWERS :


Col H — Contract Age (years): =DATEDIF(C2,TODAY(),"Y")
Col I — Contract Age (months): =DATEDIF(C2,TODAY(),"M")
Col J — Contract Age (days): =DATEDIF(C2,TODAY(),"D")
Col K — Expiry Date: =EDATE(C2,D2)
Col L — Days to Expiry: =K2-TODAY()
Col M — Status: =IF(K2<TODAY(),"EXPIRED","ACTIVE")
Col N — Days since Last Review: =TODAY()-E2
Col O — Next Review Due: =EDATE(E2,6)
Col P — Review Status: =IF(TODAY()>O2,"Review Overdue","OK")
Col Q — Expiry Month: =TEXT(K2,"MMM-YYYY")
Col R — Yearfrac: =ROUND(YEARFRAC(C2,TODAY()),1)


ANS .


<img width="3033" height="2091" alt="Picture 43" src="https://github.com/user-attachments/assets/7014875e-a859-4f19-a983-3ea121ef6296" />



Summary below data:
— Count Active: =COUNTIF(M2:M81,"ACTIVE")
— Count Expired: =COUNTIF(M2:M81,"EXPIRED")
— Count Review Overdue: =COUNTIF(P2:P81,"Review Overdue")
— Average age months: =AVERAGE(I2:I81)

Revision: CF Expired=Red row | Days to Expiry below 90=Orange | Sort Days to Expiry smallest first


ANS .


<img width="3033" height="2091" alt="Picture 43" src="https://github.com/user-attachments/assets/7014875e-a859-4f19-a983-3ea121ef6296" />
