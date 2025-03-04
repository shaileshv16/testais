::: mermaid
 graph TD;
 Customer[Customer] -->|Data Split Request| SS[Service Section];
Customer-->|Data Split Request| Mrk[Marketing];
SS-->TR([Ticket rising in Birse]);
TR-->|Ticket| CS[Customer Support Manager];
CS-->|Intimation| Mrk;
Mrk-->|PO| PS([ Transfer PO sheet])
PS-->TS[Technical Support];
TS-->|Assignment| TA[Technical Admin];
TA-->|Study| DB([Splitting Database<br>C1])
DB-->DS([Splitting database and restore<br> splitted database]);
DS-->ID([Update Implementation date<br> to PO sheet]);
ID-->Mrk1[Marketing];
DS-->|Data Split| Customer;
:::

**Checklist**

**C1:**
1. Customer Notification
2. Lock existing database
3. Backup existing database
4. set database to read only
5. Disable SMS configuration
6. Local backup restoration
7. Run split script
8. Verify script execution

