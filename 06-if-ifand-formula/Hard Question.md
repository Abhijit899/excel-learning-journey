**Business Question Answer in 1 line**

A SAP MM consultant needs to mark a PO as "Priority" only if PO Amount is above ₹200000 AND Delivery Status is "Delayed" — not if only one of those two is true. Which exact formula structure, combining two functions from today, solves this correctly?   if + AND Formula 


ANSWER : 


Use IF + AND — =IF(AND(PO Amount>200000,Delivery Status="Delayed"),"Priority","").




---



