Mini Project — Procurement Data Cleaning + Analysis 100 rows


Scenario: You are a junior SAP consultant. You received raw procurement data exported from SAP — it has duplicates, combined columns, and needs What-If analysis for budget planning.

Do all of the following:

1. Paste data in Sheet 1, rename it "Raw Data"
2. Make a copy of Sheet 1 → rename copy "Cleaned Data"
3. On Cleaned Data sheet — Remove Duplicates based on PO ID column. Note how many removed.
4. Column C has "Vendor, Category" combined — Text to Columns (comma delimiter) → split into Vendor and Category columns
5. Flash Fill: Column F has dates as "DD-MM-YYYY" — create new column extracting only the Year using Flash Fill (type 2026 for first row, Ctrl+E)
6. Add column "Tax Amount" = PO Amount × 18%
7. Add column "Total with Tax" = PO Amount + Tax Amount
8. Goal Seek: Find what PO Amount for PO6001 makes Total with Tax exactly ₹1,00,000. Set cell = that row's Total with Tax formula, To value = 100000, By changing = PO Amount cell
9. Create Sheet 2 named "Summary" with formulas only:
   — Total PO Amount: SUM
   — Total Tax Amount: SUM
   — Total with Tax: SUM
   — Count of unique POs: COUNTA
   — Highest PO Amount: MAX
10. Apply Conditional Formatting on Total with Tax column: above ₹1,50,000 = Red, below ₹50,000 = Green


QUESTION DATA :

PO ID	Month	Vendor, Category	Region	Qty	Order Date	Unit Price (₹)	PO Amount (₹)	Delivery Status
PO6001	January	Tata Steel, Raw Material	North	5	01-01-2026	2000	25000	Delivered
PO6002	February	Reliance Industries, Packaging	South	10	05-01-2026	5000	42000	Pending
PO6003	March	Bajaj Auto, Machinery	East	15	10-01-2026	8000	85000	Delayed
PO6004	April	Mahindra, Chemicals	West	20	15-01-2026	15000	120000	Delivered
PO6005	May	Wipro, IT Equipment	North	25	20-01-2026	25000	67000	Delivered
PO6006	June	HUL, Office Supplies	South	30	25-01-2026	1200	18000	Pending
PO6007	July	Asian Paints, Logistics	East	2	01-02-2026	45000	95000	Delayed
PO6008	August	Godrej, Utilities	West	8	05-02-2026	3500	38000	Delivered
PO6009	September	L&T, Raw Material	North	12	10-02-2026	6500	72000	Pending
PO6010	October	BHEL, Packaging	South	50	15-02-2026	12000	15000	Delayed
PO6011	November	Cipla, Machinery	East	5	20-02-2026	2000	110000	Delivered
PO6012	December	Maruti, Chemicals	West	10	25-02-2026	5000	55000	Pending
PO6013	January	Hero, IT Equipment	North	15	01-03-2026	8000	28000	Delayed
PO6014	February	Titan, Office Supplies	South	20	05-03-2026	15000	88000	Delivered
PO6015	March	Nestle, Logistics	East	25	10-03-2026	25000	145000	Delivered
PO6016	April	Britannia, Utilities	West	30	15-03-2026	1200	32000	Pending
PO6017	May	Infosys, Raw Material	North	2	20-03-2026	45000	76000	Delayed
PO6018	June	ITC, Packaging	South	8	25-03-2026	3500	22000	Delivered
PO6019	July	ONGC, Machinery	East	12	01-04-2026	6500	98000	Pending
PO6020	August	Sun Pharma, Chemicals	West	50	05-04-2026	12000	48000	Delayed
PO6021	September	Tata Steel, Raw Material	North	5	10-04-2026	2000	35000	Delivered
PO6022	October	Reliance Industries, Packaging	South	10	15-04-2026	5000	62000	Pending
PO6023	November	Bajaj Auto, Machinery	East	15	20-04-2026	8000	105000	Delayed
PO6024	December	Mahindra, Chemicals	West	20	25-04-2026	15000	44000	Delivered
PO6025	January	Wipro, IT Equipment	North	25	01-05-2026	25000	78000	Delivered
PO6026	February	HUL, Office Supplies	South	30	05-05-2026	1200	19000	Pending
PO6027	March	Asian Paints, Logistics	East	2	10-05-2026	45000	91000	Delayed
PO6028	April	Godrej, Utilities	West	8	15-05-2026	3500	56000	Delivered
PO6029	May	L&T, Raw Material	North	12	20-05-2026	6500	33000	Pending
PO6030	June	BHEL, Packaging	South	50	25-05-2026	12000	115000	Delayed
PO6031	July	Cipla, Machinery	East	5	01-06-2026	2000	27000	Delivered
PO6032	August	Maruti, Chemicals	West	10	05-06-2026	5000	83000	Pending
PO6033	September	Hero, IT Equipment	North	15	10-06-2026	8000	47000	Delayed
PO6034	October	Titan, Office Supplies	South	20	15-06-2026	15000	130000	Delivered
PO6035	November	Nestle, Logistics	East	25	20-06-2026	25000	60000	Delivered
PO6036	December	Britannia, Utilities	West	30	25-06-2026	1200	24000	Pending
PO6037	January	Infosys, Raw Material	North	2	01-07-2026	45000	99000	Delayed
PO6038	February	ITC, Packaging	South	8	05-07-2026	3500	41000	Delivered
PO6039	March	ONGC, Machinery	East	12	10-07-2026	6500	70000	Pending
PO6040	April	Sun Pharma, Chemicals	West	50	15-07-2026	12000	16000	Delayed
PO6041	May	Tata Steel, Raw Material	North	5	20-07-2026	2000	108000	Delivered
PO6042	June	Reliance Industries, Packaging	South	10	25-07-2026	5000	52000	Pending
PO6043	July	Bajaj Auto, Machinery	East	15	01-08-2026	8000	29000	Delayed
PO6044	August	Mahindra, Chemicals	West	20	05-08-2026	15000	86000	Delivered
PO6045	September	Wipro, IT Equipment	North	25	10-08-2026	25000	140000	Delivered
PO6046	October	HUL, Office Supplies	South	30	15-08-2026	1200	37000	Pending
PO6047	November	Asian Paints, Logistics	East	2	20-08-2026	45000	74000	Delayed
PO6048	December	Godrej, Utilities	West	8	25-08-2026	3500	21000	Delivered
PO6049	January	L&T, Raw Material	North	12	01-09-2026	6500	96000	Pending
PO6050	February	BHEL, Packaging	South	50	05-09-2026	12000	45000	Delayed
PO6051	March	Cipla, Machinery	East	5	10-09-2026	2000	31000	Delivered
PO6052	April	Maruti, Chemicals	West	10	15-09-2026	5000	118000	Pending
PO6053	May	Hero, IT Equipment	North	15	20-09-2026	8000	58000	Delayed
PO6054	June	Titan, Office Supplies	South	20	25-09-2026	15000	26000	Delivered
PO6055	July	Nestle, Logistics	East	25	01-10-2026	25000	103000	Delivered
PO6056	August	Britannia, Utilities	West	30	05-10-2026	1200	45000	Pending
PO6057	September	Infosys, Raw Material	North	2	10-10-2026	45000	82000	Delayed
PO6058	October	ITC, Packaging	South	8	15-10-2026	3500	67000	Delivered
PO6059	November	ONGC, Machinery	East	12	20-10-2026	6500	120000	Pending
PO6060	December	Sun Pharma, Chemicals	West	50	25-10-2026	12000	28000	Delayed
PO6061	January	Tata Steel, Raw Material	North	5	01-11-2026	2000	95000	Delivered
PO6062	February	Reliance Industries, Packaging	South	10	05-11-2026	5000	38000	Pending
PO6063	March	Bajaj Auto, Machinery	East	15	10-11-2026	8000	150000	Delayed
PO6064	April	Mahindra, Chemicals	West	20	15-11-2026	15000	55000	Delivered
PO6065	May	Wipro, IT Equipment	North	25	20-11-2026	25000	73000	Delivered
PO6066	June	HUL, Office Supplies	South	30	25-11-2026	1200	18000	Pending
PO6067	July	Asian Paints, Logistics	East	2	01-12-2026	45000	105000	Delayed
PO6068	August	Godrej, Utilities	West	8	05-12-2026	3500	42000	Delivered
PO6069	September	L&T, Raw Material	North	12	10-12-2026	6500	31000	Pending
PO6070	October	BHEL, Packaging	South	50	15-12-2026	12000	88000	Delayed
PO6071	November	Cipla, Machinery	East	5	20-12-2026	2000	140000	Delivered
PO6072	December	Maruti, Chemicals	West	10	25-12-2026	5000	76000	Pending
PO6073	January	Hero, IT Equipment	North	15	01-01-2027	8000	22000	Delayed
PO6074	February	Titan, Office Supplies	South	20	05-01-2027	15000	98000	Delivered
PO6075	March	Nestle, Logistics	East	25	10-01-2027	25000	48000	Delivered
PO6076	April	Britannia, Utilities	West	30	15-01-2027	1200	35000	Pending
PO6077	May	Infosys, Raw Material	North	2	20-01-2027	45000	115000	Delayed
PO6078	June	ITC, Packaging	South	8	25-01-2027	3500	62000	Delivered
PO6079	July	ONGC, Machinery	East	12	01-02-2027	6500	27000	Pending
PO6080	August	Sun Pharma, Chemicals	West	50	05-02-2027	12000	91000	Delayed
PO6081	September	Tata Steel, Raw Material	North	5	10-02-2027	2000	57000	Delivered
PO6082	October	Reliance Industries, Packaging	South	10	15-02-2027	5000	130000	Pending
PO6083	November	Bajaj Auto, Machinery	East	15	20-02-2027	8000	44000	Delayed
PO6084	December	Mahindra, Chemicals	West	20	25-02-2027	15000	78000	Delivered
PO6085	January	Wipro, IT Equipment	North	25	01-03-2027	25000	19000	Delivered
PO6086	February	HUL, Office Supplies	South	30	05-03-2027	1200	108000	Pending
PO6087	March	Asian Paints, Logistics	East	2	10-03-2027	45000	52000	Delayed
PO6088	April	Godrej, Utilities	West	8	15-03-2027	3500	33000	Delivered
PO6089	May	L&T, Raw Material	North	12	20-03-2027	6500	86000	Pending
PO6090	June	BHEL, Packaging	South	50	25-03-2027	12000	145000	Delayed
PO6091	July	Cipla, Machinery	East	5	01-04-2027	2000	37000	Delivered
PO6092	August	Maruti, Chemicals	West	10	05-04-2027	5000	74000	Pending
PO6093	September	Hero, IT Equipment	North	15	10-04-2027	8000	24000	Delayed
PO6094	October	Titan, Office Supplies	South	20	15-04-2027	15000	99000	Delivered
PO6095	November	Nestle, Logistics	East	25	20-04-2027	25000	41000	Delivered
PO6096	December	Britannia, Utilities	West	30	25-04-2027	1200	70000	Pending
PO6097	January	Infosys, Raw Material	North	2	01-05-2027	45000	16000	Delayed
PO6098	February	ITC, Packaging	South	8	05-05-2027	3500	112000	Delivered
PO6099	March	ONGC, Machinery	East	12	10-05-2027	6500	58000	Pending
PO6100	April	Sun Pharma, Chemicals	West	50	15-05-2027	12000	29000	Delayed



ANSWERS :


1. Paste data in Sheet 1, rename it "Raw Data"
Ans.
<img width="1549" height="841" alt="Screenshot 2026-04-06 173106" src="https://github.com/user-attachments/assets/a512273a-7359-4cf6-9b26-92b14916845f" />

2. Make a copy of Sheet 1 → rename copy "Cleaned Data"
Ans.
<img width="900" height="2400" alt="CLEANED DATA" src="https://github.com/user-attachments/assets/4fc409e4-74f9-4a7b-8c25-a903463757b2" />

3. On Cleaned Data sheet — Remove Duplicates based on PO ID column. Note how many removed.
Ans.
<img width="900" height="2400" alt="CLEANED DATA" src="https://github.com/user-attachments/assets/3a76f7b2-6bec-46fe-97dd-8d137be96e91" />

4. Column C has "Vendor, Category" combined — Text to Columns (comma delimiter) → split into Vendor and Category columns
Ans.
<img width="881" height="2400" alt="Picture 1" src="https://github.com/user-attachments/assets/8d84df82-9d79-4c4d-aee4-1766508749dd" />

5. Flash Fill: Column F has dates as "DD-MM-YYYY" — create new column extracting only the Year using Flash Fill (type 2026 for first row, Ctrl+E)
Ans.
<img width="961" height="2425" alt="Picture 2" src="https://github.com/user-attachments/assets/707c72df-c684-409f-8f87-0a6d7743929b" />

6. Add column "Tax Amount" = PO Amount × 18%
Ans.
<img width="1041" height="2425" alt="Picture 3" src="https://github.com/user-attachments/assets/4413da10-8178-4032-8fc2-e1ec1b97d811" />

7. Add column "Total with Tax" = PO Amount + Tax Amount
Ans.
<img width="1041" height="2425" alt="Picture 3" src="https://github.com/user-attachments/assets/a6cac02c-7642-4495-a69f-e9ced19d8d85" />

8. Goal Seek: Find what PO Amount for PO6001 makes Total with Tax exactly ₹1,00,000. Set cell = that row's Total with Tax formula, To value = 100000, By changing = PO Amount cell
Ans.
<img width="1109" height="2425" alt="Picture 4" src="https://github.com/user-attachments/assets/38dc77c5-b0ea-4178-9167-9484e4982230" />

9. Create Sheet 2 named "Summary" with formulas only:
   — Total PO Amount: SUM
   — Total Tax Amount: SUM
   — Total with Tax: SUM
   — Count of unique POs: COUNTA
   — Highest PO Amount: MAX

Answer. 
<img width="1691" height="2425" alt="Picture 5" src="https://github.com/user-attachments/assets/36836c92-581e-439b-a965-fac5ae1a4f94" />

10. Apply Conditional Formatting on Total with Tax column: above ₹1,50,000 = Red, below ₹50,000 = Green
 Ans.
<img width="1691" height="2425" alt="Picture 5" src="https://github.com/user-attachments/assets/10f04b0a-a29c-4f15-94f6-f8724891b3d4" />
