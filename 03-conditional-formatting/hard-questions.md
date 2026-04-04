## Question 1 — Multiple Rules on Same Column
A sales manager has 200 rows of sales data in column B.
He wants:
- Red fill for sales below 10000
- Yellow fill for sales between 10000 and 50000
- Green fill for sales above 50000

Task: Apply all 3 rules on column B.
What happens when two rules apply to the same cell?
How do you control which rule has priority?


### My Answer:

Cell value = 85

Rule 1 → above 80 → green ✅ this applies
Rule 2 → above 60 → yellow (ignored)
Rule 3 → below 40 → red (ignored)

Green fill applies because Excel checks rules
from top to bottom and stops at the first match.
Rule 1 matches first so green wins.

If I reverse the order and put Rule 2 on top:
Rule 1 → above 60 → yellow ✅ now this applies
Because 85 is also above 60 — yellow would win.

Conclusion: Rule ORDER matters in Conditional
Formatting. Top rule always has highest priority.
You can change order in:
Home → Conditional Formatting → Manage Rules
Then use the up/down arrows to reorder.

---

## Question 2 — Entire Row Highlighting

A teacher has marks of 50 students in 5 subjects.
She wants the entire ROW of any student whose
average is below 40 to turn red automatically.


### My Answer:
No student's average was below 40 in original data.
Changed Arjun's marks to show the rule working.

Formula used: =AVERAGE($B2:$E2)<40

Steps:
1. Selected range A2:E6
2. New Rule → Use a formula
3. Entered =AVERAGE($B2:$E2)<40
4. Set fill color to Red
5. Entire row turns red when average drops below 40


<img width="915" height="369" alt="Screenshot 2026-03-19 120304" src="https://github.com/user-attachments/assets/43187281-8fc2-480e-a060-789516de72d8" />


---


## Question 3 — Icon Sets

A company tracks monthly sales targets for 10 salespeople.
- Arrow up → achieved target
- Arrow sideways → within 10% of target
- Arrow down → missed target by more than 10%

Which Conditional Formatting option handles this?
Write the exact steps to apply it.

Use this data:
| Salesperson | Sales Amount |
|---|---|
| Riya | 95000 |
| Arjun | 48000 |
| Sneha | 12000 |
| Priya | 67000 |
| Rohan | 31000 |
| Amit | 88000 |
| Pooja | 25000 |
| Vikram | 72000 |
| Neha | 15000 |
| Rahul | 56000 |

### My Answer:
Applied Icon Sets → 3 Arrows Colored on Sales column.

Excel automatically divided data into 3 groups:
- Green arrow up → top performers (88000 and above)
- Yellow arrow sideways → average performers (56000-87000)
- Red arrow down → low performers (below 56000)

Steps:
1. Selected B2:B11 (sales amount column)
2. Home → Conditional Formatting → Icon Sets
3. Selected 3 Arrows Colored
4. Excel automatically assigned icons based on value range


<img width="483" height="665" alt="Screenshot 2026-03-19 124847" src="https://github.com/user-attachments/assets/abeedb6f-3f53-40df-8935-85bf60da0d69" />


---


Hard Q1 — Vendor Invoice Data 55 rows

Apply Conditional Formatting on this data:

1. Highlight Invoice Amount > ₹80,000 → Red fill
2. Highlight Invoice Amount < ₹30,000 → Green fill
3. Highlight Payment Status = "Pending" → Yellow fill
4. Apply Data Bars on the Invoice Amount column
5. Use Top 10% rule on Invoice Amount — what color does Excel apply by default?

Answers:

1. Highlight Invoice Amount > ₹80,000 → Red fill
Ans. <img width="701" height="1344" alt="Picture1" src="https://github.com/user-attachments/assets/104094b1-ae25-4e63-87de-971e0e0183cd" />

2. Highlight Invoice Amount < ₹30,000 → Green fill
Ans. <img width="701" height="1345" alt="Picture 4" src="https://github.com/user-attachments/assets/a4318f76-6ffc-4145-8846-b96ea7a358d8" />

3. Highlight Payment Status = "Pending" → Yellow fill
Ans. <img width="701" height="1345" alt="Picture 5" src="https://github.com/user-attachments/assets/19945f5e-fdac-4248-a935-e9ef267a4af1" />

4.  Apply Data Bars on the Invoice Amount column
Ans. <img width="701" height="1345" alt="Picture 6" src="https://github.com/user-attachments/assets/b1e01bc2-f8c7-43c6-933d-3f494af0366a" />

5. Use Top 10% rule on Invoice Amount — what color does Excel apply by default?
Ans.<img width="701" height="1345" alt="Picture 7" src="https://github.com/user-attachments/assets/75fd022b-817a-42cd-8d15-889abb05e0c4" />



