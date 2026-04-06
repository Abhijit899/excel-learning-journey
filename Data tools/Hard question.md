Hard Q1 — Vendor Master Data Cleaning 55 rows

This dataset has intentional duplicates and combined text columns. Use Data Tools to clean it:

1. Remove duplicate rows based on Vendor ID column — how many duplicates were removed?
2. Column D has "City, State" combined — use Text to Columns (delimiter = comma) to split into two separate columns: City and State
3. Column E has full vendor names in "LASTNAME, Firstname" format — use Flash Fill to create a new column with "Firstname LASTNAME" format. Type the first example manually, then Ctrl+E
4. After cleaning, use COUNTA to count how many unique vendors remain
5. Use Remove Duplicates on Vendor Name column — how many additional duplicates found?

QUESTION DATA :

Vendor ID	Vendor Name	Category	Location (City,State)	Contact Person	Rating
V1001	SHARMA, Rajesh	Raw Material	Mumbai,Maharashtra	9800000000	3
V1002	NAIR, Priya	Packaging	Delhi,Delhi	9800000007	4
V1003	MEHTA, Rajan	Machinery	Pune,Maharashtra	9800000014	5
V1004	JOSHI, Sneha	Chemicals	Chennai,Tamil Nadu	9800000021	4
V1005	PATIL, Karan	IT Equipment	Bangalore,Karnataka	9800000028	3
V1006	RAO, Divya	Office Supplies	Hyderabad,Telangana	9800000035	5
V1007	KUMAR, Mohit	Logistics	Ahmedabad,Gujarat	9800000042	4
V1008	SINGH, Ritika	Utilities	Kolkata,West Bengal	9800000049	3
V1009	PILLAI, Suresh	Raw Material	Jaipur,Rajasthan	9800000056	4
V1010	MENON, Pooja	Packaging	Surat,Gujarat	9800000063	5
V1011	VERMA, Arun	Machinery	Mumbai,Maharashtra	9800000070	3
V1012	IYER, Meena	Chemicals	Delhi,Delhi	9800000077	4
V1013	GUPTA, Tarun	IT Equipment	Pune,Maharashtra	9800000084	5
V1014	DESAI, Swati	Office Supplies	Chennai,Tamil Nadu	9800000091	4
V1015	BOSE, Nikhil	Logistics	Bangalore,Karnataka	9800000098	3
V1016	SHAH, Leena	Utilities	Hyderabad,Telangana	9800000105	5
V1017	NAIR, Deepak	Raw Material	Ahmedabad,Gujarat	9800000112	4
V1018	RAO, Anita	Packaging	Kolkata,West Bengal	9800000119	3
V1019	JOSHI, Rahul	Machinery	Jaipur,Rajasthan	9800000126	4
V1020	PATIL, Kavita	Chemicals	Surat,Gujarat	9800000133	5
V1021	SHARMA, Rajesh	IT Equipment	Mumbai,Maharashtra	9800000140	3
V1022	NAIR, Priya	Office Supplies	Delhi,Delhi	9800000147	4
V1023	MEHTA, Rajan	Logistics	Pune,Maharashtra	9800000154	5
V1024	JOSHI, Sneha	Utilities	Chennai,Tamil Nadu	9800000161	4
V1025	PATIL, Karan	Raw Material	Bangalore,Karnataka	9800000168	3
V1026	RAO, Divya	Packaging	Hyderabad,Telangana	9800000175	5
V1027	KUMAR, Mohit	Machinery	Ahmedabad,Gujarat	9800000182	4
V1028	SINGH, Ritika	Chemicals	Kolkata,West Bengal	9800000189	3
V1029	PILLAI, Suresh	IT Equipment	Jaipur,Rajasthan	9800000196	4
V1030	MENON, Pooja	Office Supplies	Surat,Gujarat	9800000203	5
V1031	VERMA, Arun	Logistics	Mumbai,Maharashtra	9800000210	3
V1032	IYER, Meena	Utilities	Delhi,Delhi	9800000217	4
V1033	GUPTA, Tarun	Raw Material	Pune,Maharashtra	9800000224	5
V1034	DESAI, Swati	Packaging	Chennai,Tamil Nadu	9800000231	4
V1035	BOSE, Nikhil	Machinery	Bangalore,Karnataka	9800000238	3
V1036	SHAH, Leena	Chemicals	Hyderabad,Telangana	9800000245	5
V1037	NAIR, Deepak	IT Equipment	Ahmedabad,Gujarat	9800000252	4
V1038	RAO, Anita	Office Supplies	Kolkata,West Bengal	9800000259	3
V1039	JOSHI, Rahul	Logistics	Jaipur,Rajasthan	9800000266	4
V1040	PATIL, Kavita	Utilities	Surat,Gujarat	9800000273	5
V1041	SHARMA, Rajesh	Raw Material	Mumbai,Maharashtra	9800000280	3
V1042	NAIR, Priya	Packaging	Delhi,Delhi	9800000287	4
V1043	MEHTA, Rajan	Machinery	Pune,Maharashtra	9800000294	5
V1044	JOSHI, Sneha	Chemicals	Chennai,Tamil Nadu	9800000301	4
V1045	PATIL, Karan	IT Equipment	Bangalore,Karnataka	9800000308	3
V1003	MEHTA, Rajan	Machinery	Pune,Maharashtra	9800000014	5
V1006	RAO, Divya	Office Supplies	Hyderabad,Telangana	9800000035	5
V1009	PILLAI, Suresh	Raw Material	Jaipur,Rajasthan	9800000056	4
V1013	GUPTA, Tarun	IT Equipment	Pune,Maharashtra	9800000084	5
V1018	RAO, Anita	Packaging	Kolkata,West Bengal	9800000119	3
V1021	SHARMA, Rajesh	IT Equipment	Mumbai,Maharashtra	9800000140	3
V1026	RAO, Divya	Packaging	Hyderabad,Telangana	9800000175	5
V1032	IYER, Meena	Utilities	Delhi,Delhi	9800000217	4
V1039	JOSHI, Rahul	Logistics	Jaipur,Rajasthan	9800000266	4
V1043	MEHTA, Rajan	Machinery	Pune,Maharashtra	9800000294	5

Answers:

1. Remove duplicate rows based on Vendor ID column — how many duplicates were removed?
Ans.
<img width="947" height="1331" alt="Picture 1" src="https://github.com/user-attachments/assets/e7f151e6-24d1-4f77-b8cd-21fd341f92d5" />

2. Column D has "City, State" combined — use Text to Columns (delimiter = comma) to split into two separate columns: City and State
Ans.
<img width="901" height="1331" alt="Picture 2" src="https://github.com/user-attachments/assets/0f3513aa-96b7-4131-8248-311960306bbd" />

3. Column E has full vendor names in "LASTNAME, Firstname" format — use Flash Fill to create a new column with "Firstname LASTNAME" format. Type the first example manually, then Ctrl+E
Ans.
<img width="650" height="1331" alt="Picture 3" src="https://github.com/user-attachments/assets/352d1fe9-fc95-42a8-a064-79dedf1c56ad" />

4. After cleaning, use COUNTA to count how many unique vendors remain
Ans.
<img width="797" height="1331" alt="Picture 4" src="https://github.com/user-attachments/assets/1933688e-48b2-4125-9bf0-bad7986d6709" />

5. Use Remove Duplicates on Vendor Name column — how many additional duplicates found?
Ans.
<img width="669" height="1331" alt="Picture 5" src="https://github.com/user-attachments/assets/ea979e86-ecb3-4842-81c2-6681967dc6e8" />



---


Hard Q2 — Sales What-If Analysis 55 rows

Use this sales data for What-If Analysis:

1. Add a new column "Commission Amount" = Sales Amount × 8%
2. Add "Net Sales" = Sales Amount − Commission Amount
3. Goal Seek: In a separate cell, write =SUM of all Net Sales. Use Goal Seek to find what single Sales Amount value (for Rep R201) would make Total Net Sales exactly ₹40,00,000. Set cell = Total Net Sales formula, To value = 4000000, By changing cell = R201 sales amount
4. Data Table: Create a one-variable data table showing Net Sales for R201 at these commission rates: 5%, 6%, 7%, 8%, 9%, 10%, 11%, 12%
5. After Goal Seek — press Ctrl+Z to restore original value


QUESTION DATA :

Rep ID	Rep Name	Region	Product	Month	Sales Amount (₹)	Units Sold
R201	Amit Shah	North	Laptop	January	82000	5
R202	Priya Nair	South	Mobile	February	61000	8
R203	Rajan Mehta	East	Chair	March	90000	12
R204	Sneha Joshi	West	Table	April	45000	15
R205	Karan Patil	North	Shirt	May	77000	20
R206	Divya Rao	South	Shoes	June	95000	25
R207	Mohit Kumar	East	Fridge	July	53000	30
R208	Ritika Singh	West	Wardrobe	August	88000	10
R209	Suresh Pillai	North	Laptop	September	40000	18
R210	Pooja Menon	South	Mobile	October	72000	22
R211	Arun Verma	East	Chair	November	67000	5
R212	Meena Iyer	West	Table	December	84000	8
R213	Tarun Gupta	North	Shirt	January	59000	12
R214	Swati Desai	South	Shoes	February	91000	15
R215	Nikhil Bose	East	Fridge	March	76000	20
R216	Leena Shah	West	Wardrobe	April	48000	25
R217	Deepak Nair	North	Laptop	May	83000	30
R218	Anita Rao	South	Mobile	June	69000	10
R219	Rahul Joshi	East	Chair	July	93000	18
R220	Kavita Patil	West	Table	August	55000	22
R221	Amit Shah	North	Shirt	September	71000	5
R222	Priya Nair	South	Shoes	October	86000	8
R223	Rajan Mehta	East	Fridge	November	49000	12
R224	Sneha Joshi	West	Wardrobe	December	92000	15
R225	Karan Patil	North	Laptop	January	63000	20
R226	Divya Rao	South	Mobile	February	57000	25
R227	Mohit Kumar	East	Chair	March	80000	30
R228	Ritika Singh	West	Table	April	74000	10
R229	Suresh Pillai	North	Shirt	May	44000	18
R230	Pooja Menon	South	Shoes	June	98000	22
R231	Arun Verma	East	Fridge	July	66000	5
R232	Meena Iyer	West	Wardrobe	August	51000	8
R233	Tarun Gupta	North	Laptop	September	87000	12
R234	Swati Desai	South	Mobile	October	75000	15
R235	Nikhil Bose	East	Chair	November	42000	20
R236	Leena Shah	West	Table	December	96000	25
R237	Deepak Nair	North	Shirt	January	58000	30
R238	Anita Rao	South	Shoes	February	64000	10
R239	Rahul Joshi	East	Fridge	March	79000	18
R240	Kavita Patil	West	Wardrobe	April	89000	22
R241	Amit Shah	North	Laptop	May	46000	5
R242	Priya Nair	South	Mobile	June	85000	8
R243	Rajan Mehta	East	Chair	July	70000	12
R244	Sneha Joshi	West	Table	August	53000	15
R245	Karan Patil	North	Shirt	September	94000	20
R246	Divya Rao	South	Shoes	October	68000	25
R247	Mohit Kumar	East	Fridge	November	47000	30
R248	Ritika Singh	West	Wardrobe	December	81000	10
R249	Suresh Pillai	North	Laptop	January	73000	18
R250	Pooja Menon	South	Mobile	February	60000	22
R251	Arun Verma	East	Chair	March	88000	5
R252	Meena Iyer	West	Table	April	77000	8
R253	Tarun Gupta	North	Shirt	May	50000	12
R254	Swati Desai	South	Shoes	June	91000	15
R255	Nikhil Bose	East	Fridge	July	65000	20


Answer :

1. Add a new column "Commission Amount" = Sales Amount × 8%
Ans.
<img width="754" height="1331" alt="Picture 6" src="https://github.com/user-attachments/assets/838e592a-39b3-4bd6-b2c8-7b667bab5bfa" />

2. Add "Net Sales" = Sales Amount − Commission Amount
Ans.
<img width="754" height="1331" alt="Picture 6" src="https://github.com/user-attachments/assets/9d5ade32-6271-4ce7-befc-eb7c05c32505" />

3. Goal Seek: In a separate cell, write =SUM of all Net Sales. Use Goal Seek to find what single Sales Amount value (for Rep R201) would make Total Net Sales exactly ₹40,00,000. Set cell = Total Net Sales formula, To value = 4000000, By changing cell = R201 sales amount
Ans.
<img width="890" height="1331" alt="Picture 7" src="https://github.com/user-attachments/assets/0746cbe4-2da8-4704-9474-8a8a0b3e025e" />


