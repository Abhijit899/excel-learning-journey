## Question 1 — Real World Multi Level Sort

| Name | Department | Salary | Joining Date | Performance Rating |
|---|---|---|---|---|
| Riya | HR | 45000 | 2019-03-15 | 4 |
| Arjun | IT | 72000 | 2018-07-22 | 5 |
| Sneha | HR | 38000 | 2021-01-10 | 3 |
| Priya | IT | 88000 | 2017-05-30 | 5 |
| Rohan | Finance | 56000 | 2020-08-14 | 4 |
| Amit | HR | 62000 | 2016-11-25 | 5 |
| Pooja | Finance | 41000 | 2022-03-07 | 2 |
| Vikram | IT | 95000 | 2015-09-18 | 5 |
| Neha | Finance | 73000 | 2019-06-29 | 4 |
| Rahul | HR | 51000 | 2020-12-01 | 3 |

Sort in this exact order:
1. Department A to Z
2. Within each department — Performance Rating highest first
3. Within same rating — Joining Date oldest first


### My Answer:
Steps using Custom Sort:
1. Select entire data A1:E11
2. Data → Sort → Custom Sort
3. Level 1 → Sort by Department → A to Z
4. Add Level → Sort by Performance Rating → Largest to Smallest
5. Add Level → Sort by Joining Date → Oldest to Newest
6. Click OK



<img width="920" height="602" alt="Screenshot 2026-03-19 211602" src="https://github.com/user-attachments/assets/51f0ec5f-18a9-4711-85e6-c619cf5a42cf" />

---

## Question 2 — Trick Question

| Month | Sales |
|---|---|
| January | 45000 |
| February | 62000 |
| March | 45000 |
| April | 88000 |
| May | 31000 |
| June | 75000 |
| July | 45000 |
| August | 56000 |
| September | 92000 |
| October | 38000 |
| November | 45000 |
| December | 71000 |

You sort by Sales Amount descending.
January, March, July and November all have
exactly the same sales — 45000.
What does Excel do with those 4 rows?
How can you control which one appears first?



<img width="359" height="599" alt="Screenshot 2026-03-19 213348" src="https://github.com/user-attachments/assets/9dd4dcbf-f5d0-4775-a9ff-d6dfe118081d" />

---
Q3.

Sales Rep Data 55 rows

Perform the following sorts one by one (undo after each before doing the next):

1. Sort by Sales Amount — Largest to Smallest
2. Sort by Rep Name — A to Z
3. Multi-level sort: First by Region (A to Z), then by Sales Amount (Largest to Smallest)
4. Multi-level sort: First by Product (A to Z), then by Month (A to Z), then by Sales (Largest to Smallest)
5. Add a column "Rank" manually (1 to 55) before sorting so you can restore original order — then sort by Sales descending and verify Rank column is still intact

Rep ID	Rep Name	Region	Product	Month	Sales Amount (₹)	Units Sold
R101	Amit Shah	North	Laptop	January	82000	5
R102	Priya Nair	South	Mobile	February	61000	8
R103	Rajan Mehta	East	Chair	March	90000	12
R104	Sneha Joshi	West	Table	April	45000	15
R105	Karan Patil	North	Shirt	May	77000	20
R106	Divya Rao	South	Shoes	June	95000	25
R107	Mohit Kumar	East	Fridge	July	53000	30
R108	Ritika Singh	West	Wardrobe	August	88000	10
R109	Suresh Pillai	North	Laptop	September	40000	18
R110	Pooja Menon	South	Mobile	October	72000	22
R111	Arun Verma	East	Chair	November	67000	5
R112	Meena Iyer	West	Table	December	84000	8
R113	Tarun Gupta	North	Shirt	January	59000	12
R114	Swati Desai	South	Shoes	February	91000	15
R115	Nikhil Bose	East	Fridge	March	76000	20
R116	Leena Shah	West	Wardrobe	April	48000	25
R117	Deepak Nair	North	Laptop	May	83000	30
R118	Anita Rao	South	Mobile	June	69000	10
R119	Rahul Joshi	East	Chair	July	93000	18
R120	Kavita Patil	West	Table	August	55000	22
R121	Sanjay Mehta	North	Shirt	September	71000	5
R122	Lakshmi Nair	South	Shoes	October	86000	8
R123	Vijay Kumar	East	Fridge	November	49000	12
R124	Rekha Singh	West	Wardrobe	December	92000	15
R125	Manoj Pillai	North	Laptop	January	63000	20
R126	Sunita Menon	South	Mobile	February	57000	25
R127	Harish Verma	East	Chair	March	80000	30
R128	Geeta Iyer	West	Table	April	74000	10
R129	Naveen Gupta	North	Shirt	May	44000	18
R130	Poonam Desai	South	Shoes	June	98000	22
R131	Amit Shah	East	Fridge	July	66000	5
R132	Priya Nair	West	Wardrobe	August	51000	8
R133	Rajan Mehta	North	Laptop	September	87000	12
R134	Sneha Joshi	South	Mobile	October	75000	15
R135	Karan Patil	East	Chair	November	42000	20
R136	Divya Rao	West	Table	December	96000	25
R137	Mohit Kumar	North	Shirt	January	58000	30
R138	Ritika Singh	South	Shoes	February	64000	10
R139	Suresh Pillai	East	Fridge	March	79000	18
R140	Pooja Menon	West	Wardrobe	April	89000	22
R141	Arun Verma	North	Laptop	May	46000	5
R142	Meena Iyer	South	Mobile	June	85000	8
R143	Tarun Gupta	East	Chair	July	70000	12
R144	Swati Desai	West	Table	August	53000	15
R145	Nikhil Bose	North	Shirt	September	94000	20
R146	Leena Shah	South	Shoes	October	68000	25
R147	Deepak Nair	East	Fridge	November	47000	30
R148	Anita Rao	West	Wardrobe	December	81000	10
R149	Rahul Joshi	North	Laptop	January	73000	18
R150	Kavita Patil	South	Mobile	February	60000	22
R151	Sanjay Mehta	East	Chair	March	88000	5
R152	Lakshmi Nair	West	Table	April	77000	8
R153	Vijay Kumar	North	Shirt	May	50000	12
R154	Rekha Singh	South	Shoes	June	91000	15
R155	Manoj Pillai	East	Fridge	July	65000	20


Answer : 

1. Sort by Sales Amount — Largest to Smallest
Ans.<img width="571" height="1369" alt="Picture 6" src="https://github.com/user-attachments/assets/d9cbe5f2-68f3-4b8d-af0b-8fe78090032b" />

2. Sort by Rep Name — A to Z
Ans. <img width="571" height="1369" alt="Picture 7" src="https://github.com/user-attachments/assets/2457a5bf-aecd-44ef-9f3b-c1564d3856fd" />

3. Multi-level sort: First by Region (A to Z), then by Sales Amount (Largest to Smallest)
Ans. <img width="571" height="1369" alt="Picture 8" src="https://github.com/user-attachments/assets/086bfae6-4615-462b-8a0b-db9773d2a572" />

4. Multi-level sort: First by Product (A to Z), then by Month (A to Z), then by Sales (Largest to Smallest)
Ans. <img width="571" height="1369" alt="Picture 9" src="https://github.com/user-attachments/assets/3895cea0-f6bf-4f60-bc6a-a708263b881f" />

5. Add a column "Rank" manually (1 to 55) before sorting so you can restore original order — then sort by Sales descending and verify Rank column is still intact
Ans. <img width="641" height="1369" alt="Picture 12" src="https://github.com/user-attachments/assets/707a0f41-625e-466b-a15c-0b80d8f5eca5" />
