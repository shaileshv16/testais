::: mermaid
 graph TD;
 SP[Service Person] -->|Expense details| UTB([Uploading travelling<br> expense in birse app]);
UTB-->|Expense details| VI[Visit In Charge];
VI-->|Check| IOF{If any<br> observations found?};
IOF-->|Yes| SP;
IOF-->|No| VRD([Verifying and reviewing<br> the expense details <br>and confirming it<br> C1]); 
VRD-->|Expense details| CSM[Customer Support Manager];
CSM-->|Check| OF{If any<br> observations found?};
OF-->|Yes| VI;
OF-->|No| VAD([Verifying and approves<br> the expense details]);
VAD-->|Expense details| FM[Finance Manager];
FM-->|Check| IAOF{If any<br>observations found?};
IAOF-->|Yes| OF;
IAOF-->|No| PPSP([Process the Payment<br> to the Service Person<br> C2]);
:::
**Checklist**

**C1:**
1. Check the Check in and check out time
2. Check working hours
3. Check the total travelling hours
4. Check the expense amount
5. Check the Claim details


**C2:**
1. Check travelling details
2. Check travelling hours
3. Check working hours



