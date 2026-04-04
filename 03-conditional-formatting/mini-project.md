Mini Project — Procurement Dashboard Prep 100 rows

Scenario: You are a junior SAP consultant at a manufacturing company. Your manager gives you raw purchase order data and asks you to visually flag issues before the monthly review meeting.

Apply ALL of the following on this dataset:

1. PO Amount > ₹1,00,000 → Red fill (high value orders need approval)
2. PO Amount < ₹10,000 → Grey fill (petty purchases)
3. Delivery Status = "Delayed" → Orange fill on entire row
4. Delivery Status = "Pending" → Yellow fill on entire row
5. Data Bars on PO Amount column
6. Color Scale on Quantity Ordered (green = high, red = low)
7. Top 5 PO Amounts → highlight with bold border using Top/Bottom rule
8. Custom formula: highlight rows where Vendor Rating < 3 → Light red fill
   Formula: =$G2<3

PO ID	Month	Vendor Name	Category	Qty	Unit Price (₹)	Vendor Rating	PO Amount (₹)	Delivery Status
PO3001	January	Tata Steel	Raw Material	5	2000	1	10000	Delivered
PO3002	February	Reliance	Packaging	10	5000	2	50000	Pending
PO3003	March	Bajaj Electricals	Machinery	15	8000	3	120000	Delayed
PO3004	April	Mahindra Logistics	Chemicals	20	15000	3	300000	Delivered
PO3005	May	Wipro Infra	IT Equipment	25	25000	4	625000	Delivered
PO3006	June	HUL Supplies	Office Supplies	30	1200	4	36000	Pending
PO3007	July	Asian Paints	Logistics	2	45000	4	90000	Delayed
PO3008	August	Godrej Industries	Utilities	8	3500	5	28000	Delivered
PO3009	September	L&T Materials	Raw Material	12	6500	5	78000	Delivered
PO3010	October	BHEL Parts	Packaging	50	12000	5	600000	Pending
PO3011	November	Cipla Chemicals	Machinery	5	2000	1	10000	Delivered
PO3012	December	Maruti Parts	Chemicals	10	5000	2	50000	Pending
PO3013	January	Hero Components	IT Equipment	15	8000	3	120000	Delayed
PO3014	February	Titan Tools	Office Supplies	20	15000	3	300000	Delivered
PO3015	March	Nestle Packaging	Logistics	25	25000	4	625000	Delivered
PO3016	April	Britannia Supplies	Utilities	30	1200	4	36000	Pending
PO3017	May	Infosys IT	Raw Material	2	45000	4	90000	Delayed
PO3018	June	ITC Packaging	Packaging	8	3500	5	28000	Delivered
PO3019	July	ONGC Parts	Machinery	12	6500	5	78000	Delivered
PO3020	August	Sun Pharma	Chemicals	50	12000	5	600000	Pending
PO3021	September	Tata Steel	IT Equipment	5	2000	1	10000	Delivered
PO3022	October	Reliance	Office Supplies	10	5000	2	50000	Pending
PO3023	November	Bajaj Electricals	Logistics	15	8000	3	120000	Delayed
PO3024	December	Mahindra Logistics	Utilities	20	15000	3	300000	Delivered
PO3025	January	Wipro Infra	Raw Material	25	25000	4	625000	Delivered
PO3026	February	HUL Supplies	Packaging	30	1200	4	36000	Pending
PO3027	March	Asian Paints	Machinery	2	45000	4	90000	Delayed
PO3028	April	Godrej Industries	Chemicals	8	3500	5	28000	Delivered
PO3029	May	L&T Materials	IT Equipment	12	6500	5	78000	Delivered
PO3030	June	BHEL Parts	Office Supplies	50	12000	5	600000	Pending
PO3031	July	Cipla Chemicals	Logistics	5	2000	1	10000	Delivered
PO3032	August	Maruti Parts	Utilities	10	5000	2	50000	Pending
PO3033	September	Hero Components	Raw Material	15	8000	3	120000	Delayed
PO3034	October	Titan Tools	Packaging	20	15000	3	300000	Delivered
PO3035	November	Nestle Packaging	Machinery	25	25000	4	625000	Delivered
PO3036	December	Britannia Supplies	Chemicals	30	1200	4	36000	Pending
PO3037	January	Infosys IT	IT Equipment	2	45000	4	90000	Delayed
PO3038	February	ITC Packaging	Office Supplies	8	3500	5	28000	Delivered
PO3039	March	ONGC Parts	Logistics	12	6500	5	78000	Delivered
PO3040	April	Sun Pharma	Utilities	50	12000	5	600000	Pending
PO3041	May	Tata Steel	Raw Material	5	2000	1	10000	Delivered
PO3042	June	Reliance	Packaging	10	5000	2	50000	Pending
PO3043	July	Bajaj Electricals	Machinery	15	8000	3	120000	Delayed
PO3044	August	Mahindra Logistics	Chemicals	20	15000	3	300000	Delivered
PO3045	September	Wipro Infra	IT Equipment	25	25000	4	625000	Delivered
PO3046	October	HUL Supplies	Office Supplies	30	1200	4	36000	Pending
PO3047	November	Asian Paints	Logistics	2	45000	4	90000	Delayed
PO3048	December	Godrej Industries	Utilities	8	3500	5	28000	Delivered
PO3049	January	L&T Materials	Raw Material	12	6500	5	78000	Delivered
PO3050	February	BHEL Parts	Packaging	50	12000	5	600000	Pending
PO3051	March	Cipla Chemicals	Machinery	5	2000	1	10000	Delivered
PO3052	April	Maruti Parts	Chemicals	10	5000	2	50000	Pending
PO3053	May	Hero Components	IT Equipment	15	8000	3	120000	Delayed
PO3054	June	Titan Tools	Office Supplies	20	15000	3	300000	Delivered
PO3055	July	Nestle Packaging	Logistics	25	25000	4	625000	Delivered
PO3056	August	Britannia Supplies	Utilities	30	1200	4	36000	Pending
PO3057	September	Infosys IT	Raw Material	2	45000	4	90000	Delayed
PO3058	October	ITC Packaging	Packaging	8	3500	5	28000	Delivered
PO3059	November	ONGC Parts	Machinery	12	6500	5	78000	Delivered
PO3060	December	Sun Pharma	Chemicals	50	12000	5	600000	Pending
PO3061	January	Tata Steel	IT Equipment	5	2000	1	10000	Delivered
PO3062	February	Reliance	Office Supplies	10	5000	2	50000	Pending
PO3063	March	Bajaj Electricals	Logistics	15	8000	3	120000	Delayed
PO3064	April	Mahindra Logistics	Utilities	20	15000	3	300000	Delivered
PO3065	May	Wipro Infra	Raw Material	25	25000	4	625000	Delivered
PO3066	June	HUL Supplies	Packaging	30	1200	4	36000	Pending
PO3067	July	Asian Paints	Machinery	2	45000	4	90000	Delayed
PO3068	August	Godrej Industries	Chemicals	8	3500	5	28000	Delivered
PO3069	September	L&T Materials	IT Equipment	12	6500	5	78000	Delivered
PO3070	October	BHEL Parts	Office Supplies	50	12000	5	600000	Pending
PO3071	November	Cipla Chemicals	Logistics	5	2000	1	10000	Delivered
PO3072	December	Maruti Parts	Utilities	10	5000	2	50000	Pending
PO3073	January	Hero Components	Raw Material	15	8000	3	120000	Delayed
PO3074	February	Titan Tools	Packaging	20	15000	3	300000	Delivered
PO3075	March	Nestle Packaging	Machinery	25	25000	4	625000	Delivered
PO3076	April	Britannia Supplies	Chemicals	30	1200	4	36000	Pending
PO3077	May	Infosys IT	IT Equipment	2	45000	4	90000	Delayed
PO3078	June	ITC Packaging	Office Supplies	8	3500	5	28000	Delivered
PO3079	July	ONGC Parts	Logistics	12	6500	5	78000	Delivered
PO3080	August	Sun Pharma	Utilities	50	12000	5	600000	Pending
PO3081	September	Tata Steel	Raw Material	5	2000	1	10000	Delivered
PO3082	October	Reliance	Packaging	10	5000	2	50000	Pending
PO3083	November	Bajaj Electricals	Machinery	15	8000	3	120000	Delayed
PO3084	December	Mahindra Logistics	Chemicals	20	15000	3	300000	Delivered
PO3085	January	Wipro Infra	IT Equipment	25	25000	4	625000	Delivered
PO3086	February	HUL Supplies	Office Supplies	30	1200	4	36000	Pending
PO3087	March	Asian Paints	Logistics	2	45000	4	90000	Delayed
PO3088	April	Godrej Industries	Utilities	8	3500	5	28000	Delivered
PO3089	May	L&T Materials	Raw Material	12	6500	5	78000	Delivered
PO3090	June	BHEL Parts	Packaging	50	12000	5	600000	Pending
PO3091	July	Cipla Chemicals	Machinery	5	2000	1	10000	Delivered
PO3092	August	Maruti Parts	Chemicals	10	5000	2	50000	Pending
PO3093	September	Hero Components	IT Equipment	15	8000	3	120000	Delayed
PO3094	October	Titan Tools	Office Supplies	20	15000	3	300000	Delivered
PO3095	November	Nestle Packaging	Logistics	25	25000	4	625000	Delivered
PO3096	December	Britannia Supplies	Utilities	30	1200	4	36000	Pending
PO3097	January	Infosys IT	Raw Material	2	45000	4	90000	Delayed
PO3098	February	ITC Packaging	Packaging	8	3500	5	28000	Delivered
PO3099	March	ONGC Parts	Machinery	12	6500	5	78000	Delivered
PO3100	April	Sun Pharma	Chemicals	50	12000	5	600000	Pending

Answers :

1. PO Amount > ₹1,00,000 → Red fill (high value orders need approval)
Ans. <img width="1092" height="2425" alt="picture 8" src="https://github.com/user-attachments/assets/1991cd45-6cd9-4628-862d-c98de3f101c6" />

2. PO Amount < ₹10,000 → Grey fill (petty purchases)
Ans. <img width="1092" height="2425" alt="Picture 9" src="https://github.com/user-attachments/assets/044046c6-7616-4c82-8098-cf0296a399d5" />

3. Delivery Status = "Delayed" → Orange fill on entire row
Ans.<img width="1092" height="2425" alt="Picture 10" src="https://github.com/user-attachments/assets/22f7bcdc-a5aa-41dc-a711-2f6075a56949" />

4. Delivery Status = "Pending" → Yellow fill on entire row'
Ans. <img width="1092" height="2425" alt="Picture 1" src="https://github.com/user-attachments/assets/921ac14d-699f-4e9e-a932-3f368efeb45f" />

5.Data Bars on PO Amount column
Ans. <img width="1092" height="2425" alt="Picture 2" src="https://github.com/user-attachments/assets/1410f092-d00f-4500-817b-0b03c11c470c" />

6. Color Scale on Quantity Ordered (green = high, red = low)
Ans.<img width="1092" height="2425" alt="Picture 3" src="https://github.com/user-attachments/assets/e0da495b-d477-479b-ad70-9ecfc4fdd3ee" />

7. Top 5 PO Amounts → highlight with bold border using Top/Bottom rule
Ans. <img width="1092" height="2425" alt="Picture 4" src="https://github.com/user-attachments/assets/c5aba8f7-f8cd-4244-9a27-f1fbfdcc5f1f" />

8. Custom formula: highlight rows where Vendor Rating < 3 → Light red fill
   Formula: =$G2<3
Ans. <img width="1092" height="2425" alt="Picture 5" src="https://github.com/user-attachments/assets/0c527458-88e6-43db-8037-8cf0c2319904" />
