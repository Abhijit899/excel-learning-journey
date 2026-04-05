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
