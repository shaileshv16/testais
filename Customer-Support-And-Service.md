::: mermaid
graph TD;
  %% Customer Initiates the Process

    CUS["Customer"] -->|Call| ST
 CUS-->CC["Call Center"]

    CC -->|Service Request| ST["Service Team"]
CUS-->|service Ticket| CT

    ST -->|Service Request| CT(["Create Ticket"])

   DM["Deployment Manager"]--> |Generate Request| CT 

     CSM["Customer Support Manager"]--> |Service Request| CT 

  

    %% Visit Request Decision
CT-->VR{If Visit Request?};
    VR -->|Yes| VRP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Visit Request Process</span>"])

    VR -->|No <br>Transfer Ticket | ST

  

    %% Service Team Resolves the Ticket

    ST --> GSRT(["Give solutions<br> to resolve the ticket"])

  GSRT-->|Check| IR{If Resolved?}

    %% Resolved or Not Resolved Decision

    IR -->|Yes| USCT(["Update the status <br>and close the ticket"])

    IR -->|No| TT(["Transfer ticket to service team"])
TT-->St1[Service Team];

  

    %% Transfer Ticket Decision

    St1-->|Check| DAR{Developer assistance<br> required or bug related}

DAR-->|Yes| TD(["Transfer to development"])

    DAR -->|No| ITF{"If transfer to higher authority"}

  

    %% Developer Assistance Path

    TD --> SDT["Scrum/Development Team"]

    SDT --> AD(["Assignment to<br> development team"])

    AD --> DT["Development Team"]

    STM["Support Team"]

  STM-->GSRT;

    %% Higher Authority Transfer Path

    ITF -->|Yes| T(["Transfer Ticket"])

    ITF -->|No| R{"If resolved?"}

  

    T --> STM

    R -->|Yes| UT(["Update the status and<br> close the ticket"])

    R-->|No| CS["Customer Support Manager"]

  

    %% Final Escalation and Alternative Actions

    CS--> TAP(["Take Alternative actions<br> to the Process"])

    TAP --> End(["End"])
click VRP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/109/Visit-Request"

:::
