::: mermaid
 graph TD;
 SL[Sales] -->|Order confirmation with<br>deployment note| CSM[Customer Support Manager];
CSM-->COC([Customer Order Intimation]);
 %%COC-->|Check| IOC{Is<br> order from new Customer?};
%%IOC-->|Yes| CIA([Customer id  creations<br> in Ais center app]);
%%IOC-->|NO| CDB;
COC-->CDB([Customer details in Birse]);
DP([Deployment Process <br>to new customer]);
CDB-->|Check| DC{If<br> data conversion found?};
DC-->|Yes| DCM[Data Conversion Manager];
DC-->|No| Csm;
DCM-->DCP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Data Conversion Process</span>"]);

DCP-->Csm(Customer Support Manager);
Csm-->|Check| ION{Is order of new customer/<br> Existing customer under<br> new deployment process};
ION-->|Yes| RD([Raise Deployment Ticket]);
RD-->|Ticket| DM[Deployment Manager];
ION-->|No| RDT([Raise Deployment Ticket]);
RDT-->|Ticket| CS[Customer Support Manager];
CS-->DEC([Deployment Process to <br>existing customer]);
DEC-->|Status| FI[Finance];
DM-->DP;
DP-->|Status| FIN[Finance];
click DCP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/145/Data-Conversion-Process"



:::
