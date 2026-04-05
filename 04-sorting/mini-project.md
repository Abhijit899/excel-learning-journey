<img width="786" height="2449" alt="Picture1" src="https://github.com/user-attachments/assets/63a04039-80e7-4052-8a0d-bae2173d7387" />
Mini Project — Vendor Payment Priority Report

Scenario: You are a junior SAP consultant. Your manager needs a vendor payment priority report sorted and formatted before a review meeting tomorrow morning.

Do all of the following in order:

1. Add a serial number column (1–100) first to preserve original order
2. Sort by Payment Status using Custom Order: Overdue → Pending → Paid
3. Within each status group, sort by Invoice Amount — Largest to Smallest (multi-level)
4. Apply Conditional Formatting: Overdue = Red, Pending = Yellow, Paid = Green on Payment Status column
5. Sort by Cell Color: Red on top, Yellow next, Green last
6. Final multi-level sort: Region (A to Z) → Payment Status (custom: Overdue, Pending, Paid) → Invoice Amount (Largest to Smallest)
7. In a separate sheet called "Summary", write using formulas only:
   — Total invoice amount (SUM)
   — Highest invoice (MAX)
   — Count of entries (COUNTA)

QUESTION DATA :

Invoice ID	Vendor Name	Region	Category	Invoice Amount (₹)	Qty	Payment Status	Due Date
INV4001	Tata Steel	North	Raw Material	45000	2	Paid	10-Jan-2026
INV4002	Reliance Industries	South	Packaging	82000	5	Pending	15-Jan-2026
INV4003	Bajaj Auto	East	Machinery	120000	8	Overdue	20-Jan-2026
INV4004	Mahindra	West	Chemicals	28000	10	Paid	25-Jan-2026
INV4005	Wipro	North	IT Equipment	95000	15	Pending	30-Jan-2026
INV4006	HUL	South	Office Supplies	67000	20	Paid	05-Feb-2026
INV4007	Asian Paints	East	Logistics	150000	25	Overdue	10-Feb-2026
INV4008	Godrej	West	Utilities	38000	30	Pending	15-Feb-2026
INV4009	L&T	North	Raw Material	73000	12	Paid	20-Feb-2026
INV4010	BHEL	South	Packaging	18000	18	Overdue	25-Feb-2026
INV4011	Cipla	East	Machinery	105000	2	Paid	01-Mar-2026
INV4012	Maruti	West	Chemicals	55000	5	Pending	05-Mar-2026
INV4013	Hero	North	IT Equipment	31000	8	Overdue	10-Mar-2026
INV4014	Titan	South	Office Supplies	88000	10	Paid	15-Mar-2026
INV4015	Nestle	East	Logistics	140000	15	Pending	20-Mar-2026
INV4016	Britannia	West	Utilities	42000	20	Paid	25-Mar-2026
INV4017	Infosys	North	Raw Material	76000	25	Overdue	30-Mar-2026
INV4018	ITC	South	Packaging	22000	30	Pending	05-Apr-2026
INV4019	ONGC	East	Machinery	98000	12	Paid	10-Apr-2026
INV4020	Sun Pharma	West	Chemicals	48000	18	Overdue	15-Apr-2026
INV4021	Tata Steel	North	IT Equipment	35000	2	Paid	20-Apr-2026
INV4022	Reliance Industries	South	Office Supplies	115000	5	Pending	25-Apr-2026
INV4023	Bajaj Auto	East	Logistics	62000	8	Overdue	30-Apr-2026
INV4024	Mahindra	West	Utilities	27000	10	Paid	05-May-2026
INV4025	Wipro	North	Raw Material	91000	15	Pending	10-May-2026
INV4026	HUL	South	Packaging	57000	20	Paid	15-May-2026
INV4027	Asian Paints	East	Machinery	130000	25	Overdue	20-May-2026
INV4028	Godrej	West	Chemicals	44000	30	Pending	25-May-2026
INV4029	L&T	North	IT Equipment	78000	12	Paid	30-May-2026
INV4030	BHEL	South	Office Supplies	19000	18	Overdue	05-Jun-2026
INV4031	Cipla	East	Logistics	108000	2	Paid	10-Jun-2026
INV4032	Maruti	West	Utilities	52000	5	Pending	15-Jun-2026
INV4033	Hero	North	Raw Material	33000	8	Overdue	20-Jun-2026
INV4034	Titan	South	Packaging	86000	10	Paid	25-Jun-2026
INV4035	Nestle	East	Machinery	145000	15	Pending	30-Jun-2026
INV4036	Britannia	West	Chemicals	37000	20	Paid	05-Jul-2026
INV4037	Infosys	North	IT Equipment	74000	25	Overdue	10-Jul-2026
INV4038	ITC	South	Office Supplies	24000	30	Pending	15-Jul-2026
INV4039	ONGC	East	Logistics	99000	12	Paid	20-Jul-2026
INV4040	Sun Pharma	West	Utilities	41000	18	Overdue	25-Jul-2026
INV4041	Tata Steel	North	Raw Material	70000	2	Paid	30-Jul-2026
INV4042	Reliance Industries	South	Packaging	16000	5	Pending	05-Aug-2026
INV4043	Bajaj Auto	East	Machinery	112000	8	Overdue	10-Aug-2026
INV4044	Mahindra	West	Chemicals	58000	10	Paid	15-Aug-2026
INV4045	Wipro	North	IT Equipment	29000	15	Pending	20-Aug-2026
INV4046	HUL	South	Office Supplies	83000	20	Paid	25-Aug-2026
INV4047	Asian Paints	East	Logistics	135000	25	Overdue	30-Aug-2026
INV4048	Godrej	West	Utilities	47000	30	Pending	05-Sep-2026
INV4049	L&T	North	Raw Material	80000	12	Paid	10-Sep-2026
INV4050	BHEL	South	Packaging	21000	18	Overdue	15-Sep-2026
INV4051	Cipla	East	Machinery	96000	2	Paid	20-Sep-2026
INV4052	Maruti	West	Chemicals	45000	5	Pending	25-Sep-2026
INV4053	Hero	North	IT Equipment	26000	8	Overdue	30-Sep-2026
INV4054	Titan	South	Office Supplies	118000	10	Paid	05-Oct-2026
INV4055	Nestle	East	Logistics	60000	15	Pending	10-Oct-2026
INV4056	Britannia	West	Utilities	30000	20	Paid	15-Oct-2026
INV4057	Infosys	North	Raw Material	125000	25	Overdue	20-Oct-2026
INV4058	ITC	South	Packaging	50000	30	Pending	25-Oct-2026
INV4059	ONGC	East	Machinery	35000	12	Paid	30-Oct-2026
INV4060	Sun Pharma	West	Chemicals	92000	18	Overdue	05-Nov-2026
INV4061	Tata Steel	North	IT Equipment	40000	2	Paid	10-Nov-2026
INV4062	Reliance Industries	South	Office Supplies	68000	5	Pending	15-Nov-2026
INV4063	Bajaj Auto	East	Logistics	15000	8	Overdue	20-Nov-2026
INV4064	Mahindra	West	Utilities	102000	10	Paid	25-Nov-2026
INV4065	Wipro	North	Raw Material	54000	15	Pending	30-Nov-2026
INV4066	HUL	South	Packaging	28000	20	Paid	05-Dec-2026
INV4067	Asian Paints	East	Machinery	88000	25	Overdue	10-Dec-2026
INV4068	Godrej	West	Chemicals	144000	30	Pending	15-Dec-2026
INV4069	L&T	North	IT Equipment	38000	12	Paid	20-Dec-2026
INV4070	BHEL	South	Office Supplies	72000	18	Overdue	25-Dec-2026
INV4071	Cipla	East	Logistics	20000	2	Paid	30-Dec-2026
INV4072	Maruti	West	Utilities	110000	5	Pending	05-Jan-2027
INV4073	Hero	North	Raw Material	56000	8	Overdue	10-Jan-2027
INV4074	Titan	South	Packaging	32000	10	Paid	15-Jan-2027
INV4075	Nestle	East	Machinery	87000	15	Pending	20-Jan-2027
INV4076	Britannia	West	Chemicals	138000	20	Paid	25-Jan-2027
INV4077	Infosys	North	IT Equipment	44000	25	Overdue	30-Jan-2027
INV4078	ITC	South	Office Supplies	76000	30	Pending	05-Feb-2027
INV4079	ONGC	East	Logistics	23000	12	Paid	10-Feb-2027
INV4080	Sun Pharma	West	Utilities	97000	18	Overdue	15-Feb-2027
INV4081	Tata Steel	North	Raw Material	46000	2	Paid	20-Feb-2027
INV4082	Reliance Industries	South	Packaging	71000	5	Pending	25-Feb-2027
INV4083	Bajaj Auto	East	Machinery	17000	8	Overdue	30-Mar-2027
INV4084	Mahindra	West	Chemicals	106000	10	Paid	05-Apr-2027
INV4085	Wipro	North	IT Equipment	53000	15	Pending	10-Apr-2027
INV4086	HUL	South	Office Supplies	30000	20	Paid	15-Apr-2027
INV4087	Asian Paints	East	Logistics	84000	25	Overdue	20-Apr-2027
INV4088	Godrej	West	Utilities	142000	30	Pending	25-Apr-2027
INV4089	L&T	North	Raw Material	36000	12	Paid	30-Apr-2027
INV4090	BHEL	South	Packaging	75000	18	Overdue	05-May-2027
INV4091	Cipla	East	Machinery	25000	2	Paid	10-May-2027
INV4092	Maruti	West	Chemicals	100000	5	Pending	15-May-2027
INV4093	Hero	North	IT Equipment	49000	8	Overdue	20-May-2027
INV4094	Titan	South	Office Supplies	69000	10	Paid	25-May-2027
INV4095	Nestle	East	Logistics	18000	15	Pending	30-May-2027
INV4096	Britannia	West	Utilities	104000	20	Paid	05-Jun-2027
INV4097	Infosys	North	Raw Material	55000	25	Overdue	10-Jun-2027
INV4098	ITC	South	Packaging	31000	30	Pending	15-Jun-2027
INV4099	ONGC	East	Machinery	89000	12	Paid	20-Jun-2027
INV4100	Sun Pharma	West	Chemicals	143000	18	Overdue	



Answers :

1. Add a serial number column (1–100) first to preserve original order
Ans.
<img width="786" height="2449" alt="Picture1" src="https://github.com/user-attachments/assets/4ae451ab-d737-4ca6-9662-c7a9537e8cb9" />


2. Sort by Payment Status using Custom Order: Overdue → Pending → Paid
Ans.
<img width="786" height="2449" alt="Picture2" src="https://github.com/user-attachments/assets/cc40fa26-95cc-42f6-9a50-1471f378ff9b" />


3. Within each status group, sort by Invoice Amount — Largest to Smallest (multi-level)
Ans.
<img width="786" height="2449" alt="Picture3" src="https://github.com/user-attachments/assets/85fefa44-9df3-49ac-80a3-5fe8c1419762" />


4. Apply Conditional Formatting: Overdue = Red, Pending = Yellow, Paid = Green on Payment Status column
Ans.
<img width="786" height="2449" alt="Picture4" src="https://github.com/user-attachments/assets/a4984dee-663c-45f7-b663-a6faef2386e3" />


6. Sort by Cell Color: Red on top, Yellow next, Green last
Ans.
<img width="786" height="2449" alt="Picture5" src="https://github.com/user-attachments/assets/15ef961f-dca9-4124-aa90-5da7e982b504" />


7. Final multi-level sort: Region (A to Z) → Payment Status (custom: Overdue, Pending, Paid) → Invoice Amount (Largest to Smallest)
Ans.
<img width="786" height="2449" alt="Picture6" src="https://github.com/user-attachments/assets/4593653a-bc6b-4767-b7d0-bae69c039b6b" />


8. In a separate sheet called "Summary", write using formulas only:
   — Total invoice amount (SUM)
   — Highest invoice (MAX)
   — Count of entries (COUNTA)

Ans. 
<img width="1502" height="765" alt="Screenshot 2026-04-05 064513" src="https://github.com/user-attachments/assets/fbb5cef3-0a9a-48de-8849-dc894b16150a" />
