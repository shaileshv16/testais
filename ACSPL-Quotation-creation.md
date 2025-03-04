::: mermaid
 graph TD;
 IFB([Information from BDM]) --> MRK[Marketing];
C([Call from customer])-->MRK;
BI([Birse ticket from<br> service section])-->MRK;
MRK-->PQ([Prepare quotation and <br>send  to the customer]);
PQ-->UQ([Update the quotation details<br> in business details]);
PQ-->|Check| IPO{If<br>Customer agree to the PO,<br> Terms and conditions};
IPO-->|No| Reject([Follow Up]);
IPO-->|Yes| P([PO receive]);
P-->UIB([Update in business details and<br> PO implementation sheet]);
UIB-->CSM[Customer Support Manager];
CSM-->|Check| INC{ If <br>new customer?};
INC-->|No| UBD([Update in business details and<br> PO implementation sheet]);
INC-->|Yes| FIN[Finance];
FIN-->CAS([Create cust mast in<br> accounting software]);

CAS-->USF([Update these details in<br> Smart fin core]);
USF-->SLB([Set a link in ACSPLM: Buyer or <br> end user master]);
SLB-->R([Recovery Status]); 
:::
