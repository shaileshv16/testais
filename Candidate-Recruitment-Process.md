::: mermaid
 graph TD;
 DD[Different Department] -->|Man power <br>recruitment request| HR[HR];
HR-->DWR([Discussion with <br>respective department <br>regarding the recruitment]);
DWR-->CI([Conduct an Interview]);
CI-->|Check| ICP{If <br>the candidate Pass?};
ICP-->|Yes| SM([Send mail to the <br> Candidate with joining date]);
ICP-->|No| RC([Reject the Candidate]);
SM-->PJL([Provide joining letter,<br> required resources <br> C1]);
PJL-->CD([Candidate detail collection<br> and update the details<br> in respective fields]);
CD-->CR([Collect candidate review from the <br>respective department and update<br> that in the employee data, salary]);
CR-->END([End]);
:::

**Checklist**

**C1:**
1. Collect Candidate Photo, Aadhar card, Pan card, Account details, Mark Cards
2. Old PF details, Old ESI details(If available)
