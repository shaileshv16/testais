::: mermaid
 graph TD;
 ST[Support Tech] -->|Tech request| TSR([Tech support <br>requirement intimation]);
TSR-->DEV[Development];
DEV-->FSP([Find solution path]);
FSP-->SE([Solutions to effort]);
SE-->IR{If<br> resolved};
IR-->|Yes| RD([Release Doc]);
RD-->S[Scrum];
RD-->SUT[Support Tech];
SUT-->CUS[Customer];
IR-->|No| INTI([Intimation]);
INTI-->SUT;
INTI-->Scrum[Scrum];
TSR-->|Information| Scrum;

:::
