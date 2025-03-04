::: mermaid
 graph TD;
 MRK[Marketing] --> GPD([Get the preliminary details of<br> the deviations/requirements]);
GPD-->CDEI([Contact Developer owner/scrum <br>for the emergency information])
CDEI-->Dev[Developer];
Dev-->S([Scrum/product owner can respond<br> to mrk for their emergency information<br> regarding feasibility /<br>scope of the deviation/requirements.])
S-->MRK1[Marketing];
CDEI-->RD([Requirement / deviations details with<br> developers emergency <br>information note to Scrum])
RD-->SCRUM1[Scrum];
SCRUM1-->|Requirement Details| PE([Process efforts of  development and deployment <br> and estimation of the delivery date. also, <br>get 3rd party dependency details])

S-->GDS([Go detail study.<br> may require to contact <br>customer whenever required])
GDS-->|Developer Concerns| PE;
PE-->RAT([RAT conclusion to mrk <br>through google sheet])
RAT-->M[Marketing];
M-->Q([Quote accordingly.<br>Inform customer regarding time required<br> and 3rd party dependency details<br> wherever required to avoid <br>unhealthily pressure to the support])
Q-->G([Get the order])
G-->SUP[Support Section];
SUP-->|PO with deviation note| RPO([Receive po with <br>deviation /requirement note])
RPO-->A([Assignment to scrum]);
A--> SCRUM[Scrum];
SCRUM-->|Requirement| D[Development];
D-->GDD([Get deviation/requirement document <br>and give assignment and get<br> estimated delivery date])
GDD-->I([Intimate estimated delivery date])
I-->|Estimated Delivery Date| Scrum2[Scrum];
Scrum2-->U([Update date in google sheet]);
U-->SUP1[Support Team];
SUP1-->IC([Intimate to customer]);
IC-->Cus[Customer];
D-->RP([Release the product and<br> produce deployment documents<br> for the deviations])
RP-->|Product released with <br>deployment documents| Scr[Scrum];
Scr-->UC([Update completion detail <br>in google sheet]);
UC-->Support([Support Section]);
Support-->Dep(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Deployment Process</span>"]);

click Dep
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/119/Deployment-Process"


:::
