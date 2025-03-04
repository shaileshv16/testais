::: mermaid
 graph TD;
 Scrum[Scrum] --> |Assignment| PL[Project lead owner]

    PL --> RA([Requirement Analysis<br>C1])

    RA --> UD([Utilize detailed requirement information])

    UD --> Cus[Customer]

    UD --> Tech[Tech]

    UD --> RD[R&D]

    UD --> SME[SME]

    UD--> PPP([Prepare plan and prototype])

    PPP --> PR([Presentation and review])

    PR --> SUP[Support]

    PR --> TEST[Testers]

    PR --> MRK[MRK]

    TEST --> PD([Prepare test designs]) --> DTH[Development team head] --> ATD([Approve test designs])

    ATD --> Testers[Testers]

    PR --> |If Finalized| IF{If <br>Finalized?}

    IF -->|No| PPP

    IF -->|Yes| EST([Estimation])

    EST --> S[Scrum]

    EST --> Testers

    EST --> AWT([Assigned within team])

    AWT --> SDEP([Software developer <br>efforts process])

    SDEP --> AT([Assigned to team])

     DET[Development Team]-->SDEP

    Testers --> TD([Test as per test designs])

    TD --> ITO{If<br> test observations?}

 ITO --> |Yes| PRN([Prepare release note]) 

    PRN --> PH[Product Head]

    PH --> AP([Approve])

    AP --> Scr[Scrum]

    Scr --> P([Product Release])

AT-->TD

ITO --> |No| SDEP
:::

**Checklist**

**C1:**
1. Project goals and Scope
2. Complexity of the project
3. Functional requirement and non functional requirement




