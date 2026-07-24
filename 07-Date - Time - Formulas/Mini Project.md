Mini Project — SAP PO Delivery Tracker 120 rows
Scenario: Junior SAP MM consultant at L&T. Build a full PO delivery tracker with date formulas + revision of math and text formulas.

Sheet 1 — "PO Tracker":
Col K — Days Open: =TODAY()-B2
Col L — Lead Time: =C2-B2
Col M — Working Days: =NETWORKDAYS(B2,C2)
Col N — Payment Due: =EOMONTH(B2,1)
Col O — Days to Payment: =N2-TODAY()
Col P — Expected Delivery: =WORKDAY(B2,15)
Col Q — On Time Flag: =IF(C2<=P2,"On Time","Late")
Col R — Days Late: =IF(C2>P2,C2-P2,0)
Col S — Month Name: =TEXT(B2,"MMM-YYYY")
Col T — GST 18% (revision): =ROUND(J2*18%,2)
Col U — Total with GST (revision): =J2+T2
Col V — Vendor Clean (revision): =PROPER(TRIM(D2))

CF: Late=Red row | Days Late above 20=Bold Red | Payment Due within 7 days=Orange
Sort: Days Late largest to smallest

Sheet 2 — "Summary":
Total POs | Count On Time | Count Late | Average Lead Time | Total PO Amount | Total GST | Earliest PO | Latest PO



ANSWER :



Sheet 1 — "PO Tracker":
Col K — Days Open: =TODAY()-B2
Col L — Lead Time: =C2-B2
Col M — Working Days: =NETWORKDAYS(B2,C2)
Col N — Payment Due: =EOMONTH(B2,1)
Col O — Days to Payment: =N2-TODAY()
Col P — Expected Delivery: =WORKDAY(B2,15)
Col Q — On Time Flag: =IF(C2<=P2,"On Time","Late")
Col R — Days Late: =IF(C2>P2,C2-P2,0)
Col S — Month Name: =TEXT(B2,"MMM-YYYY")
Col T — GST 18% (revision): =ROUND(J2*18%,2)
Col U — Total with GST (revision): =J2+T2
Col V — Vendor Clean (revision): =PROPER(TRIM(D2))

CF: Late=Red row | Days Late above 20=Bold Red | Payment Due within 7 days=Orange
Sort: Days Late largest to smallest


ANS . 


<img width="2830" height="2879" alt="Picture 44" src="https://github.com/user-attachments/assets/63c2cdc7-adc3-46c0-ae8d-68416d53cdab" />



Sheet 2 — "Summary":
Total POs | Count On Time | Count Late | Average Lead Time | Total PO Amount | Total GST | Earliest PO | Latest PO

ANS .



<img width="535" height="306" alt="Screenshot 2026-07-24 125522" src="https://github.com/user-attachments/assets/0c061577-dec9-4653-9acb-613049c4a8a0" />
