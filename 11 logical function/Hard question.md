Hard Q1 — Vendor Performance 

Col I — Performance Tag: =IF(AND(G2>=4,H2="Paid"),"Top Vendor",IF(AND(G2<3,H2="Overdue"),"High Risk","Average"))
Col J — Discount Eligible: =IF(OR(G2=5,F2>=20),"Yes","No")
Col K — Priority Flag: =IF(G2>=4,"Priority 1",IF(G2=3,"Priority 2","Priority 3"))
Col L — Action Required: =IF(AND(H2="Overdue",OR(G2<3,F2<5)),"Urgent Action",IF(H2="Pending","Follow Up","Clear"))
Col M — Bonus Level: =IF(G2=5,"Gold",IF(G2=4,"Silver",IF(G2=3,"Bronze","None")))


Vendor ID	Vendor Name	Region	Category	PO Amount (₹)	Qty	Rating (1-5)	Payment Status
V101	Tata Steel	North	Raw Material	25000	2	1	Paid
V102	Reliance Industries	South	Packaging	42000	5	2	Pending
V103	Bajaj Auto	East	Machinery	85000	8	3	Overdue
V104	Mahindra	West	Chemicals	120000	10	3	Paid
V105	Wipro	North	IT Equipment	67000	15	4	Pending
V106	HUL	South	Office Supplies	18000	20	4	Paid
V107	Asian Paints	East	Logistics	95000	25	4	Overdue
V108	Godrej	West	Utilities	38000	30	5	Pending
V109	L&T	North	Raw Material	72000	12	5	Paid
V110	BHEL	South	Packaging	15000	18	5	Overdue
V111	Cipla	East	Machinery	110000	2	1	Paid
V112	Maruti	West	Chemicals	55000	5	2	Pending
V113	Hero	North	IT Equipment	28000	8	3	Overdue
V114	Titan	South	Office Supplies	88000	10	3	Paid
V115	Nestle	East	Logistics	145000	15	4	Pending
V116	Britannia	West	Utilities	32000	20	4	Paid
V117	Infosys	North	Raw Material	76000	25	4	Overdue
V118	ITC	South	Packaging	22000	30	5	Pending
V119	ONGC	East	Machinery	98000	12	5	Paid
V120	Sun Pharma	West	Chemicals	48000	18	5	Overdue
V121	Tata Steel	North	IT Equipment	35000	2	1	Paid
V122	Reliance Industries	South	Office Supplies	62000	5	2	Pending
V123	Bajaj Auto	East	Logistics	105000	8	3	Overdue
V124	Mahindra	West	Utilities	44000	10	3	Paid
V125	Wipro	North	Raw Material	78000	15	4	Pending
V126	HUL	South	Packaging	19000	20	4	Paid
V127	Asian Paints	East	Machinery	91000	25	4	Overdue
V128	Godrej	West	Chemicals	56000	30	5	Pending
V129	L&T	North	IT Equipment	33000	12	5	Paid
V130	BHEL	South	Office Supplies	115000	18	5	Overdue
V131	Cipla	East	Logistics	27000	2	1	Paid
V132	Maruti	West	Utilities	83000	5	2	Pending
V133	Hero	North	Raw Material	47000	8	3	Overdue
V134	Titan	South	Packaging	130000	10	3	Paid
V135	Nestle	East	Machinery	60000	15	4	Pending
V136	Britannia	West	Chemicals	24000	20	4	Paid
V137	Infosys	North	IT Equipment	99000	25	4	Overdue
V138	ITC	South	Office Supplies	41000	30	5	Pending
V139	ONGC	East	Logistics	70000	12	5	Paid
V140	Sun Pharma	West	Utilities	16000	18	5	Overdue
V141	Tata Steel	North	Raw Material	108000	2	1	Paid
V142	Reliance Industries	South	Packaging	52000	5	2	Pending
V143	Bajaj Auto	East	Machinery	29000	8	3	Overdue
V144	Mahindra	West	Chemicals	86000	10	3	Paid
V145	Wipro	North	IT Equipment	140000	15	4	Pending
V146	HUL	South	Office Supplies	37000	20	4	Paid
V147	Asian Paints	East	Logistics	74000	25	4	Overdue
V148	Godrej	West	Utilities	21000	30	5	Pending
V149	L&T	North	Raw Material	96000	12	5	Paid
V150	BHEL	South	Packaging	45000	18	5	Overdue
V151	Cipla	East	Machinery	31000	2	1	Paid
V152	Maruti	West	Chemicals	118000	5	2	Pending
V153	Hero	North	IT Equipment	58000	8	3	Overdue
V154	Titan	South	Office Supplies	26000	10	3	Paid
V155	Nestle	East	Logistics	103000	15	4	Pending



Answers :

Q1. Col I — Performance Tag: =IF(AND(G2>=4,H2="Paid"),"Top Vendor",IF(AND(G2<3,H2="Overdue"),"High Risk","Average"))

Ans .

<img width="1121" height="1368" alt="Picture  3" src="https://github.com/user-attachments/assets/c5f0db21-05ad-490d-b541-9ebe072e1cb0" />

Q.2 Col J — Discount Eligible: =IF(OR(G2=5,F2>=20),"Yes","No")

Ans.

<img width="1270" height="1368" alt="Picture 4" src="https://github.com/user-attachments/assets/eb16167f-6e9a-4b5c-9f8f-fbeced7eb0e0" />

3. Col K — Priority Flag: =IF(G2>=4,"Priority 1",IF(G2=3,"Priority 2","Priority 3"))

Ans. 

<img width="1377" height="1368" alt="Picture 5" src="https://github.com/user-attachments/assets/49b638c1-4c75-4202-8b69-2d9a7f984b97" />

4. Col L — Action Required: =IF(AND(H2="Overdue",OR(G2<3,F2<5)),"Urgent Action",IF(H2="Pending","Follow Up","Clear"))

Ans.

<img width="1524" height="1368" alt="Picture 6" src="https://github.com/user-attachments/assets/538f77fd-90fd-4a1f-b326-9ec0180ca919" />

5.Col M — Bonus Level: =IF(G2=5,"Gold",IF(G2=4,"Silver",IF(G2=3,"Bronze","None")))

Ans.

<img width="1632" height="1368" alt="Picture 7" src="https://github.com/user-attachments/assets/55597906-0a8b-4024-ad18-e3497569b3c6" />

---


Hard Q2 — Sales Rep Incentive Calculator 

Col H — Target Achieved: =IF(F2>=G2,"Yes","No")
Col I — Achievement %: =F2/G2*100
Col J — Incentive Slab: =IF(I2>=120,"Platinum",IF(I2>=100,"Gold",IF(I2>=80,"Silver","No Incentive")))
Col K — Incentive Amount: =IF(J2="Platinum",F2*10%,IF(J2="Gold",F2*7%,IF(J2="Silver",F2*4%,0)))
Col L — Region Bonus: =IF(OR(C2="North",C2="South"),5000,IF(OR(C2="East",C2="West"),3000,0))
Col M — Total Payout: =K2+L2
Col N — Final Status: =IF(AND(H2="Yes",I2>=100),"Eligible for Award",IF(AND(H2="No",I2<60),"Performance Review","Standard"))


Rep ID	Rep Name	Region	Product	Month	Sales Achieved (₹)	Target (₹)
R401	Amit Shah	North	Laptop	January	82000	75000
R402	Priya Nair	South	Mobile	February	61000	70000
R403	Rajan Mehta	East	Chair	March	90000	85000
R404	Sneha Joshi	West	Table	April	45000	55000
R405	Karan Patil	North	Shirt	May	77000	80000
R406	Divya Rao	South	Shoes	June	95000	90000
R407	Mohit Kumar	East	Fridge	July	53000	60000
R408	Ritika Singh	West	Wardrobe	August	88000	80000
R409	Suresh Pillai	North	Laptop	September	40000	50000
R410	Pooja Menon	South	Mobile	October	72000	75000
R411	Arun Verma	East	Chair	November	67000	70000
R412	Meena Iyer	West	Table	December	84000	80000
R413	Tarun Gupta	North	Shirt	January	59000	65000
R414	Swati Desai	South	Shoes	February	91000	85000
R415	Nikhil Bose	East	Fridge	March	76000	80000
R416	Leena Shah	West	Wardrobe	April	48000	55000
R417	Deepak Nair	North	Laptop	May	83000	80000
R418	Anita Rao	South	Mobile	June	69000	75000
R419	Rahul Joshi	East	Chair	July	93000	90000
R420	Kavita Patil	West	Table	August	55000	60000
R421	Amit Shah	North	Shirt	September	71000	75000
R422	Priya Nair	South	Shoes	October	86000	80000
R423	Rajan Mehta	East	Fridge	November	49000	55000
R424	Sneha Joshi	West	Wardrobe	December	92000	85000
R425	Karan Patil	North	Laptop	January	63000	70000
R426	Divya Rao	South	Mobile	February	57000	65000
R427	Mohit Kumar	East	Chair	March	80000	75000
R428	Ritika Singh	West	Table	April	74000	80000
R429	Suresh Pillai	North	Shirt	May	44000	50000
R430	Pooja Menon	South	Shoes	June	98000	90000
R431	Arun Verma	East	Fridge	July	66000	70000
R432	Meena Iyer	West	Wardrobe	August	51000	55000
R433	Tarun Gupta	North	Laptop	September	87000	80000
R434	Swati Desai	South	Mobile	October	75000	80000
R435	Nikhil Bose	East	Chair	November	42000	50000
R436	Leena Shah	West	Table	December	96000	90000
R437	Deepak Nair	North	Shirt	January	58000	65000
R438	Anita Rao	South	Shoes	February	64000	70000
R439	Rahul Joshi	East	Fridge	March	79000	75000
R440	Kavita Patil	West	Wardrobe	April	89000	85000
R441	Amit Shah	North	Laptop	May	46000	55000
R442	Priya Nair	South	Mobile	June	85000	80000
R443	Rajan Mehta	East	Chair	July	70000	75000
R444	Sneha Joshi	West	Table	August	53000	60000
R445	Karan Patil	North	Shirt	September	94000	90000
R446	Divya Rao	South	Shoes	October	68000	75000
R447	Mohit Kumar	East	Fridge	November	47000	55000
R448	Ritika Singh	West	Wardrobe	December	81000	80000
R449	Suresh Pillai	North	Laptop	January	73000	80000
R450	Pooja Menon	South	Mobile	February	60000	65000
R451	Arun Verma	East	Chair	March	88000	85000
R452	Meena Iyer	West	Table	April	77000	80000
R453	Tarun Gupta	North	Shirt	May	50000	60000
R454	Swati Desai	South	Shoes	June	91000	90000
R455	Nikhil Bose	East	Fridge	July	65000	70000


Answer :

Q1. Col H — Target Achieved: =IF(F2>=G2,"Yes","No")

Ans. 

<img width="1099" height="1372" alt="Picture  1" src="https://github.com/user-attachments/assets/09a4e490-327e-4e4f-9415-60b2c2f294f1" />

Q2. Col I — Achievement %: =F2/G2*100

Ans.

<img width="1254" height="1372" alt="Picture 2" src="https://github.com/user-attachments/assets/b12e8b87-e76e-4e88-bc0c-07884d994736" />

Q3. Col J — Incentive Slab: =IF(I2>=120,"Platinum",IF(I2>=100,"Gold",IF(I2>=80,"Silver","No Incentive")))

Ans.

<img width="1403" height="1372" alt="Picture 3" src="https://github.com/user-attachments/assets/b06cf057-ef42-4820-b0fc-5b23fccbe2e4" />

Q4. Col K — Incentive Amount: =IF(J2="Platinum",F2*10%,IF(J2="Gold",F2*7%,IF(J2="Silver",F2*4%,0)))

Ans. 

<img width="1588" height="1372" alt="Picture 4" src="https://github.com/user-attachments/assets/84b4c770-2dd0-417b-a111-aaa05fc95149" />

Q5. Col L — Region Bonus: =IF(OR(C2="North",C2="South"),5000,IF(OR(C2="East",C2="West"),3000,0))

Ans.

<img width="1734" height="1372" alt="Picture 5" src="https://github.com/user-attachments/assets/369b6d90-d888-4336-ada6-4122d1bf73a7" />

Q6. Col M — Total Payout: =K2+L2

Ans. 

<img width="1869" height="1372" alt="Picture 6" src="https://github.com/user-attachments/assets/7413ea0d-8905-4191-a7d9-f29a67099571" />


Q7. Col N — Final Status: =IF(AND(H2="Yes",I2>=100),"Eligible for Award",IF(AND(H2="No",I2<60),"Performance Review","Standard"))

Ans. 

<img width="2009" height="1372" alt="Picture 7" src="https://github.com/user-attachments/assets/442528fc-0de4-4900-9d68-525a3e9f9456" />


