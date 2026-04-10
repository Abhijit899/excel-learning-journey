Mini Project — Protected SAP Procurement Report 

Scenario: You are a junior SAP consultant. You built a procurement report for your manager. Before sharing it, you must protect it so no one accidentally edits formulas or deletes data — but the manager can still update the Delivery Status column.

1. Paste data in Sheet 1 — rename "PO Data"
2. Add column J "Tax Amount" = PO Amount × 18% using formula
3. Add column K "Total with Tax" = PO Amount + Tax Amount using formula
4. Unlock only column I (Delivery Status) — lock all other columns including formula columns J and K
5. Protect "PO Data" sheet — password: po123 — allow only "Select unlocked cells"
6. Verify: try editing PO Amount — should be blocked. Try editing Delivery Status — should work.
7. Create Sheet 2 named "Summary" with formulas only:
   — Total PO Amount: =SUM('PO Data'!H2:H101)
   — Total Tax: =SUM('PO Data'!J2:J101)
   — Total with Tax: =SUM('PO Data'!K2:K101)
   — Count of POs: =COUNTA('PO Data'!A2:A101)
   — Highest PO: =MAX('PO Data'!H2:H101)
8. Protect Summary sheet fully — password: sum123 — no editing at all
9. Protect Workbook — password: work123
10. Apply Conditional Formatting on Delivery Status: Delayed=Orange, Pending=Yellow, Delivered=Green
11. Set print area, landscape orientation, repeat Row 1 on every page
12. Save as: mini-project-protected-procurement.xlsx

PO ID	Month	Vendor Name	Region	Category	Qty	Unit Price (₹)	PO Amount (₹)	Delivery Status
PO7001	January	Tata Steel	North	Raw Material	5	2000	25000	Delivered
PO7002	February	Reliance Industries	South	Packaging	10	5000	42000	Pending
PO7003	March	Bajaj Auto	East	Machinery	15	8000	85000	Delayed
PO7004	April	Mahindra	West	Chemicals	20	15000	120000	Delivered
PO7005	May	Wipro	North	IT Equipment	25	25000	67000	Delivered
PO7006	June	HUL	South	Office Supplies	30	1200	18000	Pending
PO7007	July	Asian Paints	East	Logistics	2	45000	95000	Delayed
PO7008	August	Godrej	West	Utilities	8	3500	38000	Delivered
PO7009	September	L&T	North	Raw Material	12	6500	72000	Pending
PO7010	October	BHEL	South	Packaging	50	12000	15000	Delayed
PO7011	November	Cipla	East	Machinery	5	2000	110000	Delivered
PO7012	December	Maruti	West	Chemicals	10	5000	55000	Pending
PO7013	January	Hero	North	IT Equipment	15	8000	28000	Delayed
PO7014	February	Titan	South	Office Supplies	20	15000	88000	Delivered
PO7015	March	Nestle	East	Logistics	25	25000	145000	Delivered
PO7016	April	Britannia	West	Utilities	30	1200	32000	Pending
PO7017	May	Infosys	North	Raw Material	2	45000	76000	Delayed
PO7018	June	ITC	South	Packaging	8	3500	22000	Delivered
PO7019	July	ONGC	East	Machinery	12	6500	98000	Pending
PO7020	August	Sun Pharma	West	Chemicals	50	12000	48000	Delayed
PO7021	September	Tata Steel	North	IT Equipment	5	2000	35000	Delivered
PO7022	October	Reliance Industries	South	Office Supplies	10	5000	62000	Pending
PO7023	November	Bajaj Auto	East	Logistics	15	8000	105000	Delayed
PO7024	December	Mahindra	West	Utilities	20	15000	44000	Delivered
PO7025	January	Wipro	North	Raw Material	25	25000	78000	Delivered
PO7026	February	HUL	South	Packaging	30	1200	19000	Pending
PO7027	March	Asian Paints	East	Machinery	2	45000	91000	Delayed
PO7028	April	Godrej	West	Chemicals	8	3500	56000	Delivered
PO7029	May	L&T	North	IT Equipment	12	6500	33000	Pending
PO7030	June	BHEL	South	Office Supplies	50	12000	115000	Delayed
PO7031	July	Cipla	East	Logistics	5	2000	27000	Delivered
PO7032	August	Maruti	West	Utilities	10	5000	83000	Pending
PO7033	September	Hero	North	Raw Material	15	8000	47000	Delayed
PO7034	October	Titan	South	Packaging	20	15000	130000	Delivered
PO7035	November	Nestle	East	Machinery	25	25000	60000	Delivered
PO7036	December	Britannia	West	Chemicals	30	1200	24000	Pending
PO7037	January	Infosys	North	IT Equipment	2	45000	99000	Delayed
PO7038	February	ITC	South	Office Supplies	8	3500	41000	Delivered
PO7039	March	ONGC	East	Logistics	12	6500	70000	Pending
PO7040	April	Sun Pharma	West	Utilities	50	12000	16000	Delayed
PO7041	May	Tata Steel	North	Raw Material	5	2000	108000	Delivered
PO7042	June	Reliance Industries	South	Packaging	10	5000	52000	Pending
PO7043	July	Bajaj Auto	East	Machinery	15	8000	29000	Delayed
PO7044	August	Mahindra	West	Chemicals	20	15000	86000	Delivered
PO7045	September	Wipro	North	IT Equipment	25	25000	140000	Delivered
PO7046	October	HUL	South	Office Supplies	30	1200	37000	Pending
PO7047	November	Asian Paints	East	Logistics	2	45000	74000	Delayed
PO7048	December	Godrej	West	Utilities	8	3500	21000	Delivered
PO7049	January	L&T	North	Raw Material	12	6500	96000	Pending
PO7050	February	BHEL	South	Packaging	50	12000	45000	Delayed
PO7051	March	Cipla	East	Machinery	5	2000	31000	Delivered
PO7052	April	Maruti	West	Chemicals	10	5000	118000	Pending
PO7053	May	Hero	North	IT Equipment	15	8000	58000	Delayed
PO7054	June	Titan	South	Office Supplies	20	15000	26000	Delivered
PO7055	July	Nestle	East	Logistics	25	25000	103000	Delivered
PO7056	August	Britannia	West	Utilities	30	1200	45000	Pending
PO7057	September	Infosys	North	Raw Material	2	45000	82000	Delayed
PO7058	October	ITC	South	Packaging	8	3500	67000	Delivered
PO7059	November	ONGC	East	Machinery	12	6500	120000	Pending
PO7060	December	Sun Pharma	West	Chemicals	50	12000	28000	Delayed
PO7061	January	Tata Steel	North	IT Equipment	5	2000	95000	Delivered
PO7062	February	Reliance Industries	South	Office Supplies	10	5000	38000	Pending
PO7063	March	Bajaj Auto	East	Logistics	15	8000	150000	Delayed
PO7064	April	Mahindra	West	Utilities	20	15000	55000	Delivered
PO7065	May	Wipro	North	Raw Material	25	25000	73000	Delivered
PO7066	June	HUL	South	Packaging	30	1200	18000	Pending
PO7067	July	Asian Paints	East	Machinery	2	45000	105000	Delayed
PO7068	August	Godrej	West	Chemicals	8	3500	42000	Delivered
PO7069	September	L&T	North	IT Equipment	12	6500	31000	Pending
PO7070	October	BHEL	South	Office Supplies	50	12000	88000	Delayed
PO7071	November	Cipla	East	Logistics	5	2000	140000	Delivered
PO7072	December	Maruti	West	Utilities	10	5000	76000	Pending
PO7073	January	Hero	North	Raw Material	15	8000	22000	Delayed
PO7074	February	Titan	South	Packaging	20	15000	98000	Delivered
PO7075	March	Nestle	East	Machinery	25	25000	48000	Delivered
PO7076	April	Britannia	West	Chemicals	30	1200	35000	Pending
PO7077	May	Infosys	North	IT Equipment	2	45000	115000	Delayed
PO7078	June	ITC	South	Office Supplies	8	3500	62000	Delivered
PO7079	July	ONGC	East	Logistics	12	6500	27000	Pending
PO7080	August	Sun Pharma	West	Utilities	50	12000	91000	Delayed
PO7081	September	Tata Steel	North	Raw Material	5	2000	57000	Delivered
PO7082	October	Reliance Industries	South	Packaging	10	5000	130000	Pending
PO7083	November	Bajaj Auto	East	Machinery	15	8000	44000	Delayed
PO7084	December	Mahindra	West	Chemicals	20	15000	78000	Delivered
PO7085	January	Wipro	North	IT Equipment	25	25000	19000	Delivered
PO7086	February	HUL	South	Office Supplies	30	1200	108000	Pending
PO7087	March	Asian Paints	East	Logistics	2	45000	52000	Delayed
PO7088	April	Godrej	West	Utilities	8	3500	33000	Delivered
PO7089	May	L&T	North	Raw Material	12	6500	86000	Pending
PO7090	June	BHEL	South	Packaging	50	12000	145000	Delayed
PO7091	July	Cipla	East	Machinery	5	2000	37000	Delivered
PO7092	August	Maruti	West	Chemicals	10	5000	74000	Pending
PO7093	September	Hero	North	IT Equipment	15	8000	24000	Delayed
PO7094	October	Titan	South	Office Supplies	20	15000	99000	Delivered
PO7095	November	Nestle	East	Logistics	25	25000	41000	Delivered
PO7096	December	Britannia	West	Utilities	30	1200	70000	Pending
PO7097	January	Infosys	North	Raw Material	2	45000		Delayed
PO7098	February	ITC	South	Packaging	8	3500		Delivered
PO7099	March	ONGC	East	Machinery	12	6500		Pending
PO7100	April	Sun Pharma	West	Chemicals	50	12000		Delayed


Answers :


1. Paste data in Sheet 1 — rename "PO Data"
Ans.

<img width="1044" height="770" alt="Screenshot 2026-04-10 054734" src="https://github.com/user-attachments/assets/eccc8294-befe-41c1-9823-02b8d986d71b" />

2. Add column J "Tax Amount" = PO Amount × 18% using formula
Ans.

<img width="989" height="2425" alt="Picture 2" src="https://github.com/user-attachments/assets/0aec64c3-120b-41f6-99e8-4985616ddd57" />

3.  Add column K "Total with Tax" = PO Amount + Tax Amount using formula
Ans.

<img width="1076" height="2425" alt="Picture 3" src="https://github.com/user-attachments/assets/abf63591-9b24-482a-b162-8986f648612e" />

4. Unlock only column I (Delivery Status) — lock all other columns including formula columns J and K
Ans.

<img width="1445" height="785" alt="Screenshot 2026-04-10 055725" src="https://github.com/user-attachments/assets/3a2702a6-d5eb-4829-a572-feea767e6031" />

<img width="1417" height="783" alt="Screenshot 2026-04-10 055742" src="https://github.com/user-attachments/assets/45a03136-396b-44ab-9fb6-bb3f8df25a40" />

5. Protect "PO Data" sheet — password: po123 — allow only "Select unlocked cells"
Ans.

<img width="1445" height="785" alt="Screenshot 2026-04-10 055725" src="https://github.com/user-attachments/assets/f4751e76-990c-41a6-8e8a-a5e880a959cb" />

6. Verify: try editing PO Amount — should be blocked. Try editing Delivery Status — should work.
Ans.

<img width="1417" height="783" alt="Screenshot 2026-04-10 055742" src="https://github.com/user-attachments/assets/b1b51f6b-afbe-45fd-a0b9-9c5560dbcc91" />

7. Create Sheet 2 named "Summary" with formulas only:
   — Total PO Amount: =SUM('PO Data'!H2:H101)
   — Total Tax: =SUM('PO Data'!J2:J101)
   — Total with Tax: =SUM('PO Data'!K2:K101)
   — Count of POs: =COUNTA('PO Data'!A2:A101)
   — Highest PO: =MAX('PO Data'!H2:H101)

Ans. 

<img width="741" height="176" alt="Screenshot 2026-04-10 195230" src="https://github.com/user-attachments/assets/8589d05e-cde7-49de-bdfc-c058428a7bd8" />

8. Protect Summary sheet fully — password: sum123 — no editing at all

Ans.

<img width="1281" height="808" alt="Screenshot 2026-04-10 195339" src="https://github.com/user-attachments/assets/2ba0d6c3-c601-4ec9-b53c-c732a96d322d" />

9. Protect Workbook — password: work123

Ans.

<img width="1455" height="984" alt="Screenshot 2026-04-10 195534" src="https://github.com/user-attachments/assets/66df03d0-a4de-435d-a501-b15d6b5b26b5" />

10. Apply Conditional Formatting on Delivery Status: Delayed=Orange, Pending=Yellow, Delivered=Green

Ans. 

<img width="1087" height="2425" alt="Picture 4" src="https://github.com/user-attachments/assets/2d7ed619-4cc2-42f9-b630-ef665c6af1b7" />


11. Set print area, landscape orientation, repeat Row 1 on every page

Ans. 

<img width="1562" height="876" alt="Screenshot 2026-04-10 200103" src="https://github.com/user-attachments/assets/a6eb4847-9774-47e3-8277-2cf0efa1b841" />

<img width="1321" height="863" alt="Screenshot 2026-04-10 195938" src="https://github.com/user-attachments/assets/5e72c915-d47b-420e-85a0-109d53337799" />
