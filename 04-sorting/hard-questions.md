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

