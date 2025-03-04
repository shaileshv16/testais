::: mermaid
 graph TD;
 ST[Support Tech] -->|Bug Intimation| BI([Bug Intimation]);
BI-->DEV[Development];
BI-->|Intimation| SCRUM[Scrum];
DEV-->|Check| IQF{If <br>quick fixation?};
IQF-->|Yes| QF([Quick fixation]);
QF-->RD([Release Doc]);
RD-->ST1[Support Tech];
ST1-->CUS[Customer];
ST1-->UBF([Update bug fixation list]);
UBF-->GS([Get support for <br>bug fixed Reports]);
GS-->SCRUM1[Scrum];
DEV-->GS;
IQF-->|No| APS([Assignment to fix <br>permanent solution]);
APS-->|Intimation| SCRUM;
SCRUM-->|For permanent <br> fixation| APS;
QF-->|Intimation| SCRUM;
DEV-->APS;
APS-->RD;
Dev[Development]-->APS;

:::

