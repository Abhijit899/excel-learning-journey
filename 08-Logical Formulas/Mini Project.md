<img width="2792" height="2879" alt="Picture 48" src="https://github.com/user-attachments/assets/9d242c28-0d9c-49fd-ab4a-110e0de7ed0f" />Mini Project — SAP Smart PO Risk Dashboard 120 rows
Scenario: Junior SAP MM consultant at Bajaj Auto. Build a smart PO risk dashboard combining logical formulas with all revision topics.

Sheet 1 — "PO Risk Data": paste 120 rows

Logical formula columns:
Col L — Approval Level: =IF(J2>500000,"Board",IF(J2>200000,"HOD",IF(J2>100000,"Manager","Auto")))
Col M — Risk Level: =IF(AND(K2="Delayed",I2<3),"Critical",IF(OR(K2="Delayed",K2="Pending"),"Medium","Low"))
Col N — Action: =IF(AND(K2="Delayed",OR(I2<3,J2>300000)),"Escalate",IF(K2="Pending","Follow Up","OK"))
Col O — Vendor Grade: =IFS(I2=5,"A",I2=4,"B",I2=3,"C",I2<3,"D",TRUE,"Unknown")
Col P — Status: =IF(AND(K2="Delivered",L2="Paid"),"Complete",IF(OR(K2="Delayed",L2="Overdue"),"Problem","Active")
Col Q — GST Rate: =SWITCH(H2,"Raw Material",5%,"Machinery",18%,"Chemicals",18%,"IT Equipment",18%,"Packaging",12%,5%)

Revision columns:
Col R — GST Amount (Day 4): =ROUND(J2*Q2,2)
Col S — Total with GST (Day 4): =J2+R2
Col T — Days Open (Day 6): =TODAY()-B2
Col U — Overdue Flag (Day 6): =IF(TODAY()-C2>30,"Overdue","OK")
Col V — Vendor Clean (Day 5): =PROPER(TRIM(D2))

CF: Critical=Red row | Medium=Orange | Escalate=Bold Red | D Grade=Red font
Sort: Risk Level custom (Critical→Medium→Low) then Total with GST largest first

Sheet 2 — "Risk Summary":
Count Critical | Count Medium | Count Low | Count Escalate | Total PO | Total GST | Average PO | Max PO | Count Overdue



ANSWERS :



Logical formula columns:
Col L — Approval Level: =IF(J2>500000,"Board",IF(J2>200000,"HOD",IF(J2>100000,"Manager","Auto")))
Col M — Risk Level: =IF(AND(K2="Delayed",I2<3),"Critical",IF(OR(K2="Delayed",K2="Pending"),"Medium","Low"))
Col N — Action: =IF(AND(K2="Delayed",OR(I2<3,J2>300000)),"Escalate",IF(K2="Pending","Follow Up","OK"))
Col O — Vendor Grade: =IFS(I2=5,"A",I2=4,"B",I2=3,"C",I2<3,"D",TRUE,"Unknown")
Col P — Status: =IF(AND(K2="Delivered",L2="Paid"),"Complete",IF(OR(K2="Delayed",L2="Overdue"),"Problem","Active")
Col Q — GST Rate: =SWITCH(H2,"Raw Material",5%,"Machinery",18%,"Chemicals",18%,"IT Equipment",18%,"Packaging",12%,5%)


ANS . 


<img width="2112" height="2879" alt="Picture 47" src="https://github.com/user-attachments/assets/a60281ab-90f4-4884-83ce-8e40a52801e7" />


Revision columns:
Col R — GST Amount (Day 4): =ROUND(J2*Q2,2)
Col S — Total with GST (Day 4): =J2+R2
Col T — Days Open (Day 6): =TODAY()-B2
Col U — Overdue Flag (Day 6): =IF(TODAY()-C2>30,"Overdue","OK")
Col V — Vendor Clean (Day 5): =PROPER(TRIM(D2))


ANS.


<img width="2792" height="2879" alt="Picture 48" src="https://github.com/user-attachments/assets/00c5147b-2a26-4999-aa96-05b988dbc84e" />


CF: Critical=Red row | Medium=Orange | Escalate=Bold Red | D Grade=Red font
Sort: Risk Level custom (Critical→Medium→Low) then Total with GST largest first

Sheet 2 — "Risk Summary":
Count Critical | Count Medium | Count Low | Count Escalate | Total PO | Total GST | Average PO | Max PO | Count Overdue


ANS .


<img width="695" height="485" alt="Screenshot 2026-07-25 201819" src="https://github.com/user-attachments/assets/1c88a98f-5202-4688-9a0a-47cfbe8facfe" />
