Mini Project — Procurement Risk & Priority Report 

Scenario: Junior SAP consultant. Manager wants a smart report that auto-tags vendors, flags risks and calculates tax using logical formulas.

Sheet 1 — "PO Data": paste data then add:
Col J — Tax 18%: =H2*18%
Col K — Total with Tax: =H2+J2
Col L — Risk Level: =IF(AND(I2="Delayed",G2<3),"Critical",IF(OR(I2="Delayed",I2="Pending"),"Medium","Low"))
Col M — Approval: =IF(AND(H2>100000,G2<4),"Manager Approval",IF(H2>100000,"HOD Approval","Auto Approved"))
Col N — Vendor Grade: =IF(G2=5,"A",IF(G2=4,"B",IF(G2=3,"C","D")))
Col O — Action Tag: =IF(AND(I2="Delayed",OR(G2<3,H2>100000)),"Escalate",IF(I2="Pending","Chase","OK"))

CF: Critical row=Red (=$L2="Critical") | Medium row=Yellow | Manager Approval=Orange | Grade D=Red font

Sheet 2 — "Summary": Total PO | Total Tax | Total with Tax | Count Critical | Count Auto Approved | Count Grade A | MAX PO
Protect PO Data — password: logic123 | Save as: mini-project-logical-functions-procurement.xlsx

PO ID	Month	Vendor Name	Region	Category	Qty	Vendor Rating	PO Amount (₹)	Delivery Status
PO9001	January	Tata Steel	North	Raw Material	5	1	25000	Delivered
PO9002	February	Reliance Industries	South	Packaging	10	2	42000	Pending
PO9003	March	Bajaj Auto	East	Machinery	15	3	85000	Delayed
PO9004	April	Mahindra	West	Chemicals	20	3	120000	Delivered
PO9005	May	Wipro	North	IT Equipment	25	4	67000	Delivered
PO9006	June	HUL	South	Office Supplies	30	4	18000	Pending
PO9007	July	Asian Paints	East	Logistics	2	4	95000	Delayed
PO9008	August	Godrej	West	Utilities	8	5	38000	Delivered
PO9009	September	L&T	North	Raw Material	12	5	72000	Pending
PO9010	October	BHEL	South	Packaging	50	5	15000	Delayed
PO9011	November	Cipla	East	Machinery	5	1	110000	Delivered
PO9012	December	Maruti	West	Chemicals	10	2	55000	Pending
PO9013	January	Hero	North	IT Equipment	15	3	28000	Delayed
PO9014	February	Titan	South	Office Supplies	20	3	88000	Delivered
PO9015	March	Nestle	East	Logistics	25	4	145000	Delivered
PO9016	April	Britannia	West	Utilities	30	4	32000	Pending
PO9017	May	Infosys	North	Raw Material	2	4	76000	Delayed
PO9018	June	ITC	South	Packaging	8	5	22000	Delivered
PO9019	July	ONGC	East	Machinery	12	5	98000	Pending
PO9020	August	Sun Pharma	West	Chemicals	50	5	48000	Delayed
PO9021	September	Tata Steel	North	IT Equipment	5	1	35000	Delivered
PO9022	October	Reliance Industries	South	Office Supplies	10	2	62000	Pending
PO9023	November	Bajaj Auto	East	Logistics	15	3	105000	Delayed
PO9024	December	Mahindra	West	Utilities	20	3	44000	Delivered
PO9025	January	Wipro	North	Raw Material	25	4	78000	Delivered
PO9026	February	HUL	South	Packaging	30	4	19000	Pending
PO9027	March	Asian Paints	East	Machinery	2	4	91000	Delayed
PO9028	April	Godrej	West	Chemicals	8	5	56000	Delivered
PO9029	May	L&T	North	IT Equipment	12	5	33000	Pending
PO9030	June	BHEL	South	Office Supplies	50	5	115000	Delayed
PO9031	July	Cipla	East	Logistics	5	1	27000	Delivered
PO9032	August	Maruti	West	Utilities	10	2	83000	Pending
PO9033	September	Hero	North	Raw Material	15	3	47000	Delayed
PO9034	October	Titan	South	Packaging	20	3	130000	Delivered
PO9035	November	Nestle	East	Machinery	25	4	60000	Delivered
PO9036	December	Britannia	West	Chemicals	30	4	24000	Pending
PO9037	January	Infosys	North	IT Equipment	2	4	99000	Delayed
PO9038	February	ITC	South	Office Supplies	8	5	41000	Delivered
PO9039	March	ONGC	East	Logistics	12	5	70000	Pending
PO9040	April	Sun Pharma	West	Utilities	50	5	16000	Delayed
PO9041	May	Tata Steel	North	Raw Material	5	1	108000	Delivered
PO9042	June	Reliance Industries	South	Packaging	10	2	52000	Pending
PO9043	July	Bajaj Auto	East	Machinery	15	3	29000	Delayed
PO9044	August	Mahindra	West	Chemicals	20	3	86000	Delivered
PO9045	September	Wipro	North	IT Equipment	25	4	140000	Delivered
PO9046	October	HUL	South	Office Supplies	30	4	37000	Pending
PO9047	November	Asian Paints	East	Logistics	2	4	74000	Delayed
PO9048	December	Godrej	West	Utilities	8	5	21000	Delivered
PO9049	January	L&T	North	Raw Material	12	5	96000	Pending
PO9050	February	BHEL	South	Packaging	50	5	45000	Delayed
PO9051	March	Cipla	East	Machinery	5	1	31000	Delivered
PO9052	April	Maruti	West	Chemicals	10	2	118000	Pending
PO9053	May	Hero	North	IT Equipment	15	3	58000	Delayed
PO9054	June	Titan	South	Office Supplies	20	3	26000	Delivered
PO9055	July	Nestle	East	Logistics	25	4	103000	Delivered
PO9056	August	Britannia	West	Utilities	30	4	45000	Pending
PO9057	September	Infosys	North	Raw Material	2	4	82000	Delayed
PO9058	October	ITC	South	Packaging	8	5	67000	Delivered
PO9059	November	ONGC	East	Machinery	12	5	120000	Pending
PO9060	December	Sun Pharma	West	Chemicals	50	5	28000	Delayed
PO9061	January	Tata Steel	North	IT Equipment	5	1	95000	Delivered
PO9062	February	Reliance Industries	South	Office Supplies	10	2	38000	Pending
PO9063	March	Bajaj Auto	East	Logistics	15	3	150000	Delayed
PO9064	April	Mahindra	West	Utilities	20	3	55000	Delivered
PO9065	May	Wipro	North	Raw Material	25	4	73000	Delivered
PO9066	June	HUL	South	Packaging	30	4	18000	Pending
PO9067	July	Asian Paints	East	Machinery	2	4	105000	Delayed
PO9068	August	Godrej	West	Chemicals	8	5	42000	Delivered
PO9069	September	L&T	North	IT Equipment	12	5	31000	Pending
PO9070	October	BHEL	South	Office Supplies	50	5	88000	Delayed
PO9071	November	Cipla	East	Logistics	5	1	140000	Delivered
PO9072	December	Maruti	West	Utilities	10	2	76000	Pending
PO9073	January	Hero	North	Raw Material	15	3	22000	Delayed
PO9074	February	Titan	South	Packaging	20	3	98000	Delivered
PO9075	March	Nestle	East	Machinery	25	4	48000	Delivered
PO9076	April	Britannia	West	Chemicals	30	4	35000	Pending
PO9077	May	Infosys	North	IT Equipment	2	4	115000	Delayed
PO9078	June	ITC	South	Office Supplies	8	5	62000	Delivered
PO9079	July	ONGC	East	Logistics	12	5	27000	Pending
PO9080	August	Sun Pharma	West	Utilities	50	5	91000	Delayed
PO9081	September	Tata Steel	North	Raw Material	5	1	57000	Delivered
PO9082	October	Reliance Industries	South	Packaging	10	2	130000	Pending
PO9083	November	Bajaj Auto	East	Machinery	15	3	44000	Delayed
PO9084	December	Mahindra	West	Chemicals	20	3	78000	Delivered
PO9085	January	Wipro	North	IT Equipment	25	4	19000	Delivered
PO9086	February	HUL	South	Office Supplies	30	4	108000	Pending
PO9087	March	Asian Paints	East	Logistics	2	4	52000	Delayed
PO9088	April	Godrej	West	Utilities	8	5	33000	Delivered
PO9089	May	L&T	North	Raw Material	12	5	86000	Pending
PO9090	June	BHEL	South	Packaging	50	5	145000	Delayed
PO9091	July	Cipla	East	Machinery	5	1	37000	Delivered
PO9092	August	Maruti	West	Chemicals	10	2	74000	Pending
PO9093	September	Hero	North	IT Equipment	15	3	24000	Delayed
PO9094	October	Titan	South	Office Supplies	20	3	99000	Delivered
PO9095	November	Nestle	East	Logistics	25	4	41000	Delivered
PO9096	December	Britannia	West	Utilities	30	4	70000	Pending
PO9097	January	Infosys	North	Raw Material	2	4		Delayed
PO9098	February	ITC	South	Packaging	8	5		Delivered
PO9099	March	ONGC	East	Machinery	12	5		Pending
PO9100	April	Sun Pharma	West	Chemicals	50	5		Delayed


Answer :

Q1. Col J — Tax 18%: =H2*18%

Ans.

<img width="1334" height="2468" alt="Picture 8" src="https://github.com/user-attachments/assets/871033b0-6e49-4720-befd-30c03f67cdf0" />

Q2. Col K — Total with Tax: =H2+J2

Ans. 

<img width="1519" height="2468" alt="Picture 9" src="https://github.com/user-attachments/assets/53dd8865-235b-431f-ae53-22b8e43cc8a2" />

Q3. Col L — Risk Level: =IF(AND(I2="Delayed",G2<3),"Critical",IF(OR(I2="Delayed",I2="Pending"),"Medium","Low"))

Ans. 

<img width="1665" height="2468" alt="Picture 10" src="https://github.com/user-attachments/assets/a8a0652b-0eed-4780-a0cf-e677001af47a" />

Q4. Col M — Approval: =IF(AND(H2>100000,G2<4),"Manager Approval",IF(H2>100000,"HOD Approval","Auto Approved"))

Ans.

<img width="1804" height="2468" alt="Picture 11" src="https://github.com/user-attachments/assets/87de6979-0d9a-4b19-b9fa-6f1231c0bc23" />

Q5. Col N — Vendor Grade: =IF(G2=5,"A",IF(G2=4,"B",IF(G2=3,"C","D")))

Ans. 

<img width="1944" height="2468" alt="Picture 12" src="https://github.com/user-attachments/assets/7ecfa79a-b6d4-49ad-a4e5-e338ea8d0eb8" />

Q6. Col O — Action Tag: =IF(AND(I2="Delayed",OR(G2<3,H2>100000)),"Escalate",IF(I2="Pending","Chase","OK"))

Ans. 

<img width="2059" height="2468" alt="Picture 13" src="https://github.com/user-attachments/assets/6a545e5d-ffbd-4ba6-9bd5-0b904e8dfccb" />


Q7. CF: Critical row=Red (=$L2="Critical") | Medium row=Yellow | Manager Approval=Orange | Grade D=Red font

Ans. 

<img width="2059" height="2468" alt="Picture 14" src="https://github.com/user-attachments/assets/779d26c4-aa84-444c-aea8-bad726b5416d" />


Sheet 2 — "Summary": Total PO | Total Tax | Total with Tax | Count Critical | Count Auto Approved | Count Grade A | MAX PO
Protect PO Data — password: logic123 | Save as: mini-project-logical-functions-procurement.xlsx


