::: mermaid
 graph TD;
 Cust[Customer] -->|Visit request| OTS[Other than service section: <br> Mrk, Ac, Mgmt., etc.];
OTS-->|Check| ICS{If<br> the customer has <br>trouble connecting to the<br> service section};
ICS-->|Yes<br> Intimation| DM[Deployment Manager];
ICS-->|No| IC([Intimate to the customer to<br> connect the service section]);
Cust-->|Visit request| SS[Service Section];
SS-->|Request| DM;
DM-->|Deployment| VP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Visit Process</span>"]);
click VP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/108/Visit-Process"
:::
