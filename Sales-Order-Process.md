::: mermaid
 graph TD;
 MRK[MRK] -->|Lead| SL[Sales];

    SL -->URC([User Requirement<br> Collection]);

 URC-->QP([Demo and <br>Quotation Process]);

    QP -->|Check| IAR{If<br> any Additional <br>requirements?};

  Cust[Customer]-->URC;


    IAR -->|Yes| RAT[RAT];

    RAT --> RP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Requirement found<br>before order</span>"]);

    IAR -->|No| FNP([Follow<br> of negotiation Process]);

  RP-->QP;

  

    IR -->|No| Cancel([Lead Cancel Process]);

    IR{If <br>retry required?} -->|Yes| FNP;

  

    FNP -->|Check| IOF{If <br>order process <br>finalized?};

    IOF-->|No| IR;

    IOF -->|Yes| GO([Getting Order]);

  

     CUS([Customer ID <br>creation Process <br>in Ais center app]);
GO--> Sl1[Sales];
Sl1--> |Order with integration/<br>Multitenant/Individual| CUS;

    CUS-->|Order with Fin note<br> and Customer id| FIN[Finance];

    FIN -->|Order information<br> update in A/C| OIU([Order information <br>update in A/C<br> C1]);

    CUS-->|Order with Deployment note<br> and customer id| SUP[Support];

    SUP --> DP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Deployment Process</span>"]);


click DP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/119/Deployment-Process"
click RP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/156/Requirement-found-before-order"


:::

**Checklist**

**C1:**
For Existing Customer:
1. Order update in Fin core
2. Update Pigmy, AMC, I-Back up in Track

For New Customer:
1. Create cust mast in  accounting software
2. Update these details in  Smart fin core
3. Set a link in ACSPLM: Buyer or  end user master
4. Recovery Process
