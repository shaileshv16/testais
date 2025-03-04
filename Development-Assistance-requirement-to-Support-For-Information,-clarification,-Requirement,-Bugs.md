::: mermaid
 graph TD;
  ST[Support Team] --> Ticket[Ticket]

    Ticket --> IPR{If <br>Pigmy/SMS Related}

    IPR -->|Yes| PTH[Pigmy/SMS <br>Technical Head] --> VT([Verify the Ticket])

    IPR -->|No| ICR{If <br>Cloud related}

    ICR -->|Yes| CT[Cloud Technical Head] --> VT

    ICR -->|No| TH[Technical Head] --> VT

  

    VT --> GTA([Get Technical Advice])

    GTA --> SADS([Support advisor of <br>development side])

    GTA --> DS[Development Section]

    DS --> GIC([Get Information <br>for Clarification]) --> VT

  

    VT --> IS{If <br>Solution within Scope}

    IS-->|Yes| SP([Solutions Process])

    IS -->|No| Ticket[Ticket]

    Ticket --> CSM[Customer Support Manager]

    CSM --> RTD([Receives ticket in devops])

    RTD --> Scrum[Scrum]

    Scrum --> ASN([Assignment])

    ASN --> DEV[Developers]

  

    DEV--> GA([Get Assistance])

    GA -->|Assistance| Cus[Customer]

    GA -->|Assistance| Supt[Support Team]

  

    GA --> SP

    SP --> X[Scrum]

    X --> ST
:::
