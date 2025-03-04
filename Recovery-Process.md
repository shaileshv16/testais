::: mermaid
  

 graph TD;

 OR([Order with recovery note]) --> FIN[Finance];

FIN-->OD([Order details update to A/C<br>C1]);

OD-->Serst([Get service status to bills]);

CSM[Customer Service Manager]-->Serst;

Serst-->|Check| CkSerSt{ If<br> Service Status finds ok to bill};

CkSerSt-->|No <br> then wait till work further status| Serst;

CkSerSt-->|Yes| GIP([Generate invoice or Perform<br> invoice and status to customer]);

GIP-->FU([Follow up<br>C2]);

FU-->R([Recovery]);

R-->|Check| ICF{If<br>recurancy dues connect<br> to the order found};

ICF-->|No| END([End]);

R-->GR([Generate Receipt]);

GR-->CUS[Customer];

GIP-->|Invoice Or perform invoice<br> or bills| CUST[Customer];

OD-->|Due list| RPR([Regular process get on<br> time recovery duelist]);

ICF-->|Yes| RPR;
:::

**Checklist**

**C1:**

Order Update
1. One Time
2. Payables
3. Recovery note if any
4. Recurring Schedules

**C2:**
1. Call offer perform invoice/bills to recovery
2. Get support and marketing support/information if required
3. Negotiate only if mandate (If should not harm to future revenue and other customer)
4. Can do settlement whenever required with valid reason
