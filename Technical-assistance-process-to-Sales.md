::: mermaid
 graph TD;
 SUP[Support] -->|Technical assistance<br> request| SCRUM[Scrum];
SCRUM-->AP([Assignment Process]);
AP-->DEV[Developer];
DEV-->E([Efforts]);
E-->|Status| SCR[Scrum];
SCR-->WC([Work clarification]);
WC-->SUP;
:::
