Mini Project — Print-Ready Procurement Report 100 rows

Scenario: You are a junior SAP consultant. Your manager needs a print-ready procurement report to present in a board meeting tomorrow. It must look professional when printed — not like a raw Excel dump.

Do all of the following:

1. Paste data in Sheet 1, rename it "PO Data"
2. Sort by Region (A to Z), then by PO Amount (Largest to Smallest)
3. Apply Conditional Formatting: Delayed = Orange, Pending = Yellow, Delivered = Green on Delivery Status column
4. Set Print Area — data table only
5. Orientation: Landscape
6. Margins: Narrow
7. Scale: Fit width to 1 page
8. Print Titles: Row 1 repeats on every page
9. Insert page breaks between each Region so each region prints on its own page(s)
10. Header: Left = "Procurement Report Q1 2026", Right = today's date
11. Footer: Center = "Page &[Page] of &[Pages]" | Right = "Confidential"
12. Enable Gridlines for printing
13. Create Sheet 2 named "Summary" with these formulas referencing Sheet 1:
   — Total PO Amount: =SUM('PO Data'!H2:H101)
   — Highest PO: =MAX('PO Data'!H2:H101)
   — Total Entries: =COUNTA('PO Data'!A2:A101)
14. Print Preview both sheets — confirm everything looks correct

QUESTION DATA 

PO ID	Month	Vendor Name	Region	Category	Qty	Unit Price (₹)	PO Amount (₹)	Delivery Status
PO6001	January	Tata Steel	North	Raw Material	5	2000	25000	Delivered
PO6002	February	Reliance Industries	South	Packaging	10	5000	42000	Pending
PO6003	March	Bajaj Auto	East	Machinery	15	8000	85000	Delayed
PO6004	April	Mahindra	West	Chemicals	20	15000	120000	Delivered
PO6005	May	Wipro	North	IT Equipment	25	25000	67000	Delivered
PO6006	June	HUL	South	Office Supplies	30	1200	18000	Pending
PO6007	July	Asian Paints	East	Logistics	2	45000	95000	Delayed
PO6008	August	Godrej	West	Utilities	8	3500	38000	Delivered
PO6009	September	L&T	North	Raw Material	12	6500	72000	Pending
PO6010	October	BHEL	South	Packaging	50	12000	15000	Delayed
PO6011	November	Cipla	East	Machinery	5	2000	110000	Delivered
PO6012	December	Maruti	West	Chemicals	10	5000	55000	Pending
PO6013	January	Hero	North	IT Equipment	15	8000	28000	Delayed
PO6014	February	Titan	South	Office Supplies	20	15000	88000	Delivered
PO6015	March	Nestle	East	Logistics	25	25000	145000	Delivered
PO6016	April	Britannia	West	Utilities	30	1200	32000	Pending
PO6017	May	Infosys	North	Raw Material	2	45000	76000	Delayed
PO6018	June	ITC	South	Packaging	8	3500	22000	Delivered
PO6019	July	ONGC	East	Machinery	12	6500	98000	Pending
PO6020	August	Sun Pharma	West	Chemicals	50	12000	48000	Delayed
PO6021	September	Tata Steel	North	IT Equipment	5	2000	35000	Delivered
PO6022	October	Reliance Industries	South	Office Supplies	10	5000	62000	Pending
PO6023	November	Bajaj Auto	East	Logistics	15	8000	105000	Delayed
PO6024	December	Mahindra	West	Utilities	20	15000	44000	Delivered
PO6025	January	Wipro	North	Raw Material	25	25000	78000	Delivered
PO6026	February	HUL	South	Packaging	30	1200	19000	Pending
PO6027	March	Asian Paints	East	Machinery	2	45000	91000	Delayed
PO6028	April	Godrej	West	Chemicals	8	3500	56000	Delivered
PO6029	May	L&T	North	IT Equipment	12	6500	33000	Pending
PO6030	June	BHEL	South	Office Supplies	50	12000	115000	Delayed
PO6031	July	Cipla	East	Logistics	5	2000	27000	Delivered
PO6032	August	Maruti	West	Utilities	10	5000	83000	Pending
PO6033	September	Hero	North	Raw Material	15	8000	47000	Delayed
PO6034	October	Titan	South	Packaging	20	15000	130000	Delivered
PO6035	November	Nestle	East	Machinery	25	25000	60000	Delivered
PO6036	December	Britannia	West	Chemicals	30	1200	24000	Pending
PO6037	January	Infosys	North	IT Equipment	2	45000	99000	Delayed
PO6038	February	ITC	South	Office Supplies	8	3500	41000	Delivered
PO6039	March	ONGC	East	Logistics	12	6500	70000	Pending
PO6040	April	Sun Pharma	West	Utilities	50	12000	16000	Delayed
PO6041	May	Tata Steel	North	Raw Material	5	2000	108000	Delivered
PO6042	June	Reliance Industries	South	Packaging	10	5000	52000	Pending
PO6043	July	Bajaj Auto	East	Machinery	15	8000	29000	Delayed
PO6044	August	Mahindra	West	Chemicals	20	15000	86000	Delivered
PO6045	September	Wipro	North	IT Equipment	25	25000	140000	Delivered
PO6046	October	HUL	South	Office Supplies	30	1200	37000	Pending
PO6047	November	Asian Paints	East	Logistics	2	45000	74000	Delayed
PO6048	December	Godrej	West	Utilities	8	3500	21000	Delivered
PO6049	January	L&T	North	Raw Material	12	6500	96000	Pending
PO6050	February	BHEL	South	Packaging	50	12000	45000	Delayed
PO6051	March	Cipla	East	Machinery	5	2000	31000	Delivered
PO6052	April	Maruti	West	Chemicals	10	5000	118000	Pending
PO6053	May	Hero	North	IT Equipment	15	8000	58000	Delayed
PO6054	June	Titan	South	Office Supplies	20	15000	26000	Delivered
PO6055	July	Nestle	East	Logistics	25	25000	103000	Delivered
PO6056	August	Britannia	West	Utilities	30	1200	45000	Pending
PO6057	September	Infosys	North	Raw Material	2	45000	82000	Delayed
PO6058	October	ITC	South	Packaging	8	3500	67000	Delivered
PO6059	November	ONGC	East	Machinery	12	6500	120000	Pending
PO6060	December	Sun Pharma	West	Chemicals	50	12000	28000	Delayed
PO6061	January	Tata Steel	North	IT Equipment	5	2000	95000	Delivered
PO6062	February	Reliance Industries	South	Office Supplies	10	5000	38000	Pending
PO6063	March	Bajaj Auto	East	Logistics	15	8000	150000	Delayed
PO6064	April	Mahindra	West	Utilities	20	15000	55000	Delivered
PO6065	May	Wipro	North	Raw Material	25	25000	73000	Delivered
PO6066	June	HUL	South	Packaging	30	1200	18000	Pending
PO6067	July	Asian Paints	East	Machinery	2	45000	105000	Delayed
PO6068	August	Godrej	West	Chemicals	8	3500	42000	Delivered
PO6069	September	L&T	North	IT Equipment	12	6500	31000	Pending
PO6070	October	BHEL	South	Office Supplies	50	12000	88000	Delayed
PO6071	November	Cipla	East	Logistics	5	2000	140000	Delivered
PO6072	December	Maruti	West	Utilities	10	5000	76000	Pending
PO6073	January	Hero	North	Raw Material	15	8000	22000	Delayed
PO6074	February	Titan	South	Packaging	20	15000	98000	Delivered
PO6075	March	Nestle	East	Machinery	25	25000	48000	Delivered
PO6076	April	Britannia	West	Chemicals	30	1200	35000	Pending
PO6077	May	Infosys	North	IT Equipment	2	45000	115000	Delayed
PO6078	June	ITC	South	Office Supplies	8	3500	62000	Delivered
PO6079	July	ONGC	East	Logistics	12	6500	27000	Pending
PO6080	August	Sun Pharma	West	Utilities	50	12000	91000	Delayed
PO6081	September	Tata Steel	North	Raw Material	5	2000	57000	Delivered
PO6082	October	Reliance Industries	South	Packaging	10	5000	130000	Pending
PO6083	November	Bajaj Auto	East	Machinery	15	8000	44000	Delayed
PO6084	December	Mahindra	West	Chemicals	20	15000	78000	Delivered
PO6085	January	Wipro	North	IT Equipment	25	25000	19000	Delivered
PO6086	February	HUL	South	Office Supplies	30	1200	108000	Pending
PO6087	March	Asian Paints	East	Logistics	2	45000	52000	Delayed
PO6088	April	Godrej	West	Utilities	8	3500	33000	Delivered
PO6089	May	L&T	North	Raw Material	12	6500	86000	Pending
PO6090	June	BHEL	South	Packaging	50	12000	145000	Delayed
PO6091	July	Cipla	East	Machinery	5	2000	37000	Delivered
PO6092	August	Maruti	West	Chemicals	10	5000	74000	Pending
PO6093	September	Hero	North	IT Equipment	15	8000	24000	Delayed
PO6094	October	Titan	South	Office Supplies	20	15000	99000	Delivered
PO6095	November	Nestle	East	Logistics	25	25000	41000	Delivered
PO6096	December	Britannia	West	Utilities	30	1200	70000	Pending
PO6097	January	Infosys	North	Raw Material	2	45000	16000	Delayed
PO6098	February	ITC	South	Packaging	8	3500	112000	Delivered
PO6099	March	ONGC	East	Machinery	12	6500	58000	Pending
PO6100	April	Sun Pharma	West	Chemicals	50	12000	29000	Delayed



Answer :

1. Paste data in Sheet 1, rename it "PO Data"
Ans.
<img width="854" height="776" alt="Screenshot 2026-04-05 093513" src="https://github.com/user-attachments/assets/1d859973-4773-436d-bc5f-066dbfe14108" />

2. Sort by Region (A to Z), then by PO Amount (Largest to Smallest)
Ans.
<img width="859" height="2425" alt="Picture3" src="https://github.com/user-attachments/assets/5d367172-fd50-405b-92f4-d44da93c6cbf" />

3. Apply Conditional Formatting: Delayed = Orange, Pending = Yellow, Delivered = Green on Delivery Status column
Ans.
<img width="859" height="2425" alt="Picture4" src="https://github.com/user-attachments/assets/b3bb5259-62d4-4fd5-afcc-231808f5e75c" />

4. Set Print Area — data table only
Ans.
<img width="911" height="849" alt="Screenshot 2026-04-05 095402" src="https://github.com/user-attachments/assets/4e90cb97-a506-40c9-ab42-63ab4454ded4" />

5. Orientation: Landscape
Ans.
<img width="1719" height="803" alt="Screenshot 2026-04-05 095902" src="https://github.com/user-attachments/assets/e4335495-7742-4193-9ad4-16ead80efc18" />

6. Margins: Narrow
Ans.
<img width="1452" height="821" alt="Screenshot 2026-04-05 100112" src="https://github.com/user-attachments/assets/326e05d1-3403-4e0e-bc81-cd515103139a" />

7. Scale: Fit width to 1 page
Ans.
<img width="1471" height="881" alt="Screenshot 2026-04-05 100420" src="https://github.com/user-attachments/assets/90c54384-41bd-4609-8e49-50ec0c71daae" />

8. Print Titles: Row 1 repeats on every page
Ans.
<img width="935" height="799" alt="Screenshot 2026-04-05 100905" src="https://github.com/user-attachments/assets/8e4bbebe-fae0-4cda-8521-db9a1d9c6516" />
<img width="714" height="804" alt="Screenshot 2026-04-05 100910" src="https://github.com/user-attachments/assets/ad814e5a-8e7b-41b4-9c25-09a7bdac6c7a" />

9. Insert page breaks between each Region so each region prints on its own page(s)
Ans.
<img width="933" height="598" alt="Screenshot 2026-04-05 101548" src="https://github.com/user-attachments/assets/2698bb59-a262-4581-8925-06f172f02046" />
<img width="974" height="657" alt="Screenshot 2026-04-05 101558" src="https://github.com/user-attachments/assets/da3f1376-2460-4d06-afd1-5e7b744e475d" />
<img width="830" height="620" alt="Screenshot 2026-04-05 101608" src="https://github.com/user-attachments/assets/0d1c4bd2-2d4e-4cea-acb0-cf5a42004743" />
<img width="738" height="500" alt="Screenshot 2026-04-05 101615" src="https://github.com/user-attachments/assets/0a7350c3-6974-4f9b-9276-7c05a8519dda" />

10. Header: Left = "Procurement Report Q1 2026", Right = today's date
 Ans.
<img width="1047" height="670" alt="Screenshot 2026-04-05 101958" src="https://github.com/user-attachments/assets/532976c5-839a-4a3e-a280-e4a252d6f6ea" />

11. Footer: Center = "Page &[Page] of &[Pages]" | Right = "Confidential"
 Ans.
<img width="1001" height="876" alt="Screenshot 2026-04-05 102151" src="https://github.com/user-attachments/assets/a792780f-5144-4fd2-9a38-98f8fa0c9644" />

12. Enable Gridlines for printing
 Ans.
<img width="813" height="857" alt="Screenshot 2026-04-05 102254" src="https://github.com/user-attachments/assets/6350f33b-399f-4c65-91a7-9245af2ef640" />

13. Create Sheet 2 named "Summary" with these formulas referencing Sheet 1:
   — Total PO Amount: =SUM('PO Data'!H2:H101)
   — Highest PO: =MAX('PO Data'!H2:H101)
   — Total Entries: =COUNTA('PO Data'!A2:A101)
 Ans.
<img width="1187" height="2425" alt="Picture7" src="https://github.com/user-attachments/assets/ca509e4d-1ae0-4ac6-a985-f1130e129322" />

14. Print Preview both sheets — confirm everything looks correct
 Ans.
<img width="916" height="887" alt="Screenshot 2026-04-05 104115" src="https://github.com/user-attachments/assets/5457c9eb-c188-4f92-bab3-fff34332a4d4" />

<img width="850" height="852" alt="Screenshot 2026-04-05 104133" src="https://github.com/user-attachments/assets/6f0eb8a7-7131-4754-99ea-f1ad528b5f1a" />

<img width="808" height="880" alt="Screenshot 2026-04-05 104141" src="https://github.com/user-attachments/assets/d2d92c03-6124-4d9e-af6a-f479fcb9904a" />

<img width="961" height="841" alt="Screenshot 2026-04-05 104151" src="https://github.com/user-attachments/assets/7ccb9ff3-4a6b-41b1-be19-2c36b71d062a" />
