::: mermaid
 graph TD;
 DT[Department Team] -->|Request| AHD[Any head of <br>the department];
PM[Procurement Manager];
AHD-->AP([Approve]);
AP-->PM;
PM-->CR([Check the requirement<br> is accepted]);
CR-->|Check| IA{If <br>acceptable?};
IA-->|No| RI([Rejection Intimation <br>with reason]);
RI-->|Intimation| DT;
IA-->|Yes| EA{If <br>the estimated amount is below<br> the limit of dinet procurement <br>without quotation};
EA-->|Yes| DP([Do Procurement Process]);
DP-->|Intimation| AHD;
EA-->|No| IEA{If<br> the estimated  amount <br>is below  the higher approval};
IEA-->|Yes| DQP([Do Quotation Process]);
DQP-->DP;
IEA-->|No| GHA([Get higher approval]);
GHA-->Mng[Management];
Mng-->IAA{Is<br> accepted?};
%%IAA-->|Yes| IEA;%%
IAA-->|No| AHD;
IAA-->|Yes| DQP;
:::
