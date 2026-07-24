Hard Q1 — SAP PO Risk & Approval Tagging 80 rows
Add these formula columns:

Col K — Approval Required (IF):
=IF(I2>500000,"Board Approval",IF(I2>200000,"HOD Approval",IF(I2>100000,"Manager Approval","Auto Approved")))

Col L — Risk Flag (IF+AND):
=IF(AND(I2>300000,J2="Delayed"),"High Risk","Normal")

Col M — Action Tag (IF+OR):
=IF(OR(J2="Delayed",K2="Overdue"),"Immediate Action","Clear")

Col N — Vendor Grade (Nested IF):
=IF(H2>=5,"Gold",IF(H2>=4,"Silver",IF(H2>=3,"Bronze","D Grade")))

Col O — Priority Level (IFS):
=IFS(AND(I2>300000,J2="Delayed"),"P1 Critical",AND(I2>100000,J2="Delayed"),"P2 High",J2="Pending","P3 Medium",J2="Delivered","P4 Low",TRUE,"P5 Closed")

Col P — Discount Eligible (IF+OR):
=IF(OR(H2=5,I2>400000),"Yes","No")

Col Q — Combined Status (IF+AND+OR):
=IF(AND(J2="Delivered",K2="Paid"),"Complete",IF(OR(J2="Delayed",K2="Overdue"),"Problem","In Progress"))

Col R — GST Rate (SWITCH):
=SWITCH(G2,"Raw Material",5%,"Packaging",12%,"Machinery",18%,"Chemicals",18%,"IT Equipment",18%,"Office Supplies",5%,"Logistics",18%,"Utilities",5%,18%)

Col S — IFERROR test:
=IFERROR(I2/0,"Cannot Divide")

Revision: CF High Risk=Red row | P1 Critical=Orange | Gold Grade=Green | Sort by Priority Level




ANSWER :



<img width="2788" height="1925" alt="Picture 45" src="https://github.com/user-attachments/assets/26efc4fc-d931-44a3-a779-2cde9deeb061" />



---



Hard Q2 — SAP Sales Incentive Calculator 80 rows
Add these formula columns:

Col H — Target Achieved (IF):
=IF(F2>=G2,"Yes","No")

Col I — Achievement % :
=ROUND(F2/G2*100,1)

Col J — Incentive Slab (Nested IF):
=IF(I2>=120,"Platinum",IF(I2>=100,"Gold",IF(I2>=80,"Silver","No Incentive")))

Col K — Incentive % (IFS):
=IFS(J2="Platinum",10%,J2="Gold",7%,J2="Silver",4%,J2="No Incentive",0%)

Col L — Incentive Amount:
=F2*K2

Col M — Region Bonus (IF+OR):
=IF(OR(D2="North",D2="South"),5000,IF(OR(D2="East",D2="West"),3000,0))

Col N — Total Payout:
=L2+M2

Col O — Final Status (IF+AND):
=IF(AND(H2="Yes",I2>=100),"Award Eligible",IF(AND(H2="No",I2<60),"PIP",IF(H2="Yes","Standard","Below Standard")))

Col P — Star Flag (IF+AND):
=IF(AND(I2>=110,D2="North"),"North Star",IF(I2>=110,"Star Performer","Regular"))

Summary: Count Platinum | Count Gold | Total Incentive Paid | Average Achievement %

Revision: CF Platinum=Gold fill | No Incentive=Red | Sort by Achievement % descending




ANSWER :



![Uploading Picture 46.png…]()
