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
