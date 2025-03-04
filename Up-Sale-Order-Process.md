::: mermaid
 graph TD;
 USM[Up Sale Manager] -->|Strategies to <br>create up Sale| UST[Up Sale Team];
UST-->PUS([Perform Up sale <br>lead creation<br> C1]);
PUS-->FU([Follow up]);
FU-->|Check| IPR{If <br>positive response};
IPR-->|Yes| LST([Lead to sales team]);
LST-->SL[Sales Team];
SL-->LP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Lead Creation Process <br>for new Customer</span>"]);
IPR-->|No| FP([Find the possible<br> areas and return]);
FP-->GFC([Get feedback of <br>the customer]);
GFC-->|Check| INF([If <br>negative feedback?]);
INF-->|No| End([End]);
INF-->|Yes| CT([Create Ticket]);
CT-->ST[Support Team];
Cust[Customer]-->|Enquiry| IHT[Inhouse Team];
IHT-->|Intimation| USM1[Up Sale Manager];
USM1-->|Assignment| UST;
click LP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/107/Lead-Creation"
:::
**Checklist**

**C1:**

1. Get an up sale enquiry  from Customer/ support / other sources

2. Get customer list with implemented features

3. Convey by call/visit to Up sale the available services and product

4. Maintain Google sheet to update all related details like source of enquiry, dt , etc.

5. Apply right strategy to reach all the customers

6. Communicate the exact requirements and alternatives

7. Finding the scope for any other Up sale and update the information

8. Update the follow-up status to the google sheet

9. Do the needful action if any deviations are found

10. Sending quotation for the same

11. Follow up, negotiate and finalize the order

12. Regular check up the status and if the order not finalizing then mention the reason for the same

13. If the enquiry needs to be closed without order then specify the reason for the same  in the google sheet

14. Getting order

15. Monthly MIS  should be presented :
        Resources, ref dt, customer, requirements, quotation dt, quotation amt, order dt, order amt , status

16. Get the feed back and create ticket to support so that customers should have post their feedback on our product and services 
