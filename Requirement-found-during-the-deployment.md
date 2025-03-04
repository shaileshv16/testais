::: mermaid
 graph TD;

Cust[Customer]-->SS;
     SS[Support Section]
    SS --> RD([Get the preliminary details <br>of the deviations/requirements.<br> from the customer])
    RD --> REQ([Requirement / deviations details <br>with developers emergency<br> information note to RAT])
    REQ -->|Requirement| Scrum[Scrum];
Scrum-->P([Process efforts development and deployment<br> and estimation of the delivery date.<br> also, get 3rd party dependency details]);
DEV[Development]-->|Developer concern| P;
GDS([Go detail study. <br>may require to contact <br>customer whenever required]) -->DEV;
P-->RAT([RAT conclusion to mrk]);
RAT-->|RAT conclusion with efforts, <br>time, delivery date etc.| Mrk[Marketing/Up sale Team];
Mrk-->I([Inform customer regarding time required<br> and 3rd party dependency details<br> wherever required to avoid <br>unhealthily pressure to the support])
I-->|Check| B{Based on efforts analysis<br> check the quotation is require ?}
B-->|Yes| GO([Get order]);
GO-->|PO with deviation note| Support[Support Section];
Support-->R([Receive PO with deviation /<br>Requirement note]);
B-->|No| DIS([Deployment intimation to support]);
DIS-->|Deployment note<br> without PO| Support1[Support Section];
Support1-->ID([If development effort required<br> then assignment to scrum])
ID-->Scrum1[Scrum];
Scrum1-->G([Get deviation/requirement document<br> and give assignment and <br>get estimated delivery date]);
G-->IED([Intimate estimated delivery date]);
IED-->|Estimated delivery date| Sup[Support Section];
Sup-->ICED([Intimate to customer of<br> estimated delivery]);
Scrum1-->RPD([Release the product and <br>produce deployment documents<br> for the deviations])
RPD-->|Product released with <br>deployment documents| Support2[Support Section];
Support2-->Dep(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Deployment Process</span>"]);
click Dep
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/119/Deployment-Process"
:::
