::: mermaid
 graph TD;
 SUP[Customer Support Manager] -->|Data Conversion <br>Ticket| DC[Data Conversion Manager]

    DC -->|Approve| ASN([Assignment <br> C1])

    ASN --> DCT[Data Conversion Team]

    DCT --> DCP([Data Conversion Task<br> C2])

    DA -->|No| DPC([Data Conversion <br>Process Completion<br>C3 ]);
    DPC-->DCA[Data Conversion Manager];
    DCA --> DIN([Deployment Instruction<br>Note<br> C5])
    DIN --> CS[Customer Support Manager]
    CS-->DEP([Deployment Process]);
    DCP --> DA{If  <br>assistance required?}
    DA-->|Yes| DC2[Data Conversion Manager];
  DC2 -->AN([Analysis<br>C4]);
  AN-->|Check| IDA{If <br> Developer assistance<br> required?};
  IDA-->|Yes<br> Devops Ticket| Scrum[Scrum];
 Scrum --> DEV[Developers]
DEV-->|Assistance| DC2;
DC2-->|Assistance| DCT;  
DEP-->|Check| FADC{Found any data <br>conversion observation?};
FADC-->|Yes<br> Observations List| DCT
FADC-->|No| WCR([Work completion report]);
Customer[Customer]-->|Approval| WCR
WCR-->|Work completion report| Customer
WCR-->|JW Claim sheet with <br>Approved Completion Report| DCA1[Data Conversion Manager];
DCA1-->|JW Claim sheet| C[Customer Support Manager];
C-->|JW Claim Sheet| Fin[Finance] 
:::

**CHECKLIST**

**C1:**
1. Assign a specific person or team member to oversee and execute the data conversion process.

2. The assigned person checks the data type and data checking process 

3. The assigned person will act as the point of contact for all tasks and communications related to the data conversion. 

4. Conversion person received check list before conversion process start 


**C2:**

 **SERVICE PERSON CONVERTION DATA CHECK LIST BEFORE INSTALLATION**
1. Check Account Head (Control account head under group and account id Checking)

2. Check Customer data (Customer address, Village, Post in KN Or ENG ,Aadhar card number, Mobile number update)

3. Check  Opening Balance  (All Share Capital Ledger bal and dividend  all Dep control account ledger bal)
4. FD , RD , CC INTEREST schedule checking and Standing Instruction master checking 
5. FD , CC , PIGMY, RD paid interest and product updated 
6. All loan control account ledger balance
7. Loan opening Interest and penal update checking 
8. Checking loan master Repayment schedule fill or not (multiple repayment loan) 
9. All Other Sub Master Ledger balance  (If Investment , furniture master include) 
10. Checking balance sheet (Opening Balance Sheet fill or not and tally or not)
11. R AND D (Opening R AND D fill or not and tally or not )




**C3:**
1. Book begin date

2. Share master in HO or Branch
3. Customer address update in Kannada or English
4. Share link update(U_PartyMast)
5. Share capital ledger balance
6. All department control account ledger balance(Fixed deposit, Savings deposit, Recurring deposit, Pigmy deposit)
7. All loan control account ledger balance(Jewel loans, Deposit loans, MKCC loans, Surety loans)
8. All other sub master ledger balance(Suspense liability, Suspense asset)
9. Balance sheet
10. R and D
11. Standing instruction

**C4:**
1. If assistance within his limit give assistance to the team

2. Get assistance from technical expert(Rithesh)by rising devops ticket if required
3. Otherwise get assistance from developer through scrum

**C5:**

**CHECK LIST FOR SERVICE PERSON AT THE TIME OF IMPLEMENTATION**
1. All The control Account Heads Act Id assigned properly?
 
2. Customer Address, Village, Post, Caste, Aadhar No, Pan No, Mobile No are migrated properly based on their old software? 

3. All Share Individual Account wise ledger  tally 

4. All Deposit Individual Account wise ledger  tally
 
5. All Loan Individual Account wise ledger  tally 

6. Share Dividend Opening balance  tally

7. All Other Sub Accounts Ledger balance  tally 

8. FD,RD,CC interest schedules are imported correctly

9. Pigmy collector is updated correctly

10. Is Pigmy opening product  updated 

11. Is Pigmy Interest is calculating correctly

12. Is FD and CC opening paid interest  updated

13. Is Standing instruction  updated 

14. Is Loan Int, Penal int, Charges are updated properly
 
15. Is Loan Interest is calculating properly 

16. Is Loan schedules are migrated properly(check some selected accounts of all Type of loans) 

17. Is Loan Surety, DL pledge, Gold Pledge, Nominee, VL pledge are migrated? 

18. Is opening balance sheet is tally

19. Is opening R&D is tally

20. Is Old transaction is migrated





