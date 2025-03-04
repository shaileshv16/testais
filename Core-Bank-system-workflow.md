::: mermaid
 graph LR;
 A[<b>Core Banking System] -->|Has| B[<b>Smart Fincore];
style A fill:#e6aef9  ,Stroke:#01070c , stroke-width:3px;
style B fill:#c8f7e8   ,Stroke:#01070c , stroke-width:3px;
A-->|Has| C[<b>Birse FinServe];
style C fill:#c8f7e8 , Stroke:#01070c , stroke-width:3px;
A-->|Has| D[<b>Smart BC];
style D fill:#c8f7e8  ,Stroke:#01070c , stroke-width:3px;
A-->|Has| E[<b>Birse staff mobile App];
style E fill:#c8f7e8  ,Stroke:#01070c , stroke-width:3px;
A-->|Has| F[<b>Birse CRM];
style F fill:#c8f7e8  ,Stroke:#01070c , stroke-width:3px;
A-->|Has| G[<b>Sahakari mobile App];
style G fill:#c8f7e8 , Stroke:#01070c , stroke-width:3px;
A-->|Has| H[<b>Smart community App];
style H fill:#c8f7e8  ,Stroke:#01070c , stroke-width:3px;
A-->|Has| I[<b>Smart Pigmy];
style I fill:#c8f7e8  ,Stroke:#01070c , stroke-width:3px;
B-->|Used by| J[<b>Org-Staff];
style J fill:#e7eaea  ,Stroke:#01070c , stroke-width:3px;
C-->|Used by| J;
D-->|Used by| J;
E-->|Used by| J;
F-->|Used by| K[<b>Org-Management/Directors];
style K fill:#e7eaea  ,Stroke:#01070c , stroke-width:3px;
G-->|Used by| L[<b>Org-Bank Members];
style L fill:#e7eaea  ,Stroke:#01070c , stroke-width:3px;
H-->|Used by| L;
I-->|Used by| M[<b>Org-Pigmy Collectors];
style M fill:#e7eaea  ,Stroke:#01070c, stroke-width:3px;
A-->|Has| N[<b> NEFT App];
style N fill:#c8f7e8   ,Stroke:#01070c , stroke-width:3px;
N-->|Inward Fund| O[<b>Public];
style O fill:#e7eaea   ,Stroke:#01070c , stroke-width:3px;
N-->|Outward Fund| R[<b> Org-Staff];
style R fill:#e7eaea  ,Stroke:#01070c , stroke-width:3px;
A-->|Controlled by| S[<b> Ais center App];
style S fill:#e6aef9  ,Stroke:#01070c , stroke-width:3px;
S-->|Used by| T[<b>Automation Staff];
style T fill:#e7eaea  ,Stroke:#01070c , stroke-width:3px;
:::
<br>
<br>
<b>Co-Operative Society/Bank/Organization</b>: A Organization operates  with various roles and functions, comprising the following groups:<br>
<br>
<b>1. Organization Staff</b> : Employees responsible for daily operations.<br>
<br>
<b>2. Organization Members</b> : Individuals who are members of the society, participating in its benefits and services.<br>
<br>
<b>3. Organization Management/Directors</b> : Board members or directors who oversee the society’s operations and strategies.<br>
<br>
<b>4. Pigmy Collectors</b>: Individuals collecting small savings (pigmy deposits) from members on behalf of the organization.
<br>
<br>

<b>Core Banking System:</b>
The Core Banking System integrates multiple applications to facilitate banking, management, and customer services for the society. This system includes:
1. Smart Fincore App
2. Birse Finserve App
3. Smart BC App
4. Birse Staff Mobile App
5. Birse CRM App
6. Sahakari Mobile App
7. Smart Community App
8. Smart Pigmy App
9. NEFT App<br>
10. Ais center App<br>
<br>

<b>1.Smart Fincore : </B>
A banking app used by bank staff.<br>
<b>2. Birse Finserve:</b>
 Allows society staff to access WhatsApp, E-KYC, and V-KYC services for member verification and communication.<br>
<b>3. Smart BC:</b>
Smart business correspondent is a backend management application, with this application we can Monitor the business correspondent, uploading and downloading the correspondent activities. This also can be used as a bridge between BC and Offline processes of Smart Pigmy aap and Smart fincore aap.<br>
<b>4.Birse Staff Mobile App:</b>
Used by organization staff to manage their TODO List, View notifications, and generate security pins.<br>
<b>5. Birse CRM:</b>
Enables management functions for the society’s head office and related administrative sections<br>
<b>6. Sahakari Mobile App:</b>
 Available to society members for accessing society-related services.<br>
<b>7. Smart Community App:</b>
Allows the general public to enroll as members of the society.<br>
<b>8. Smart Pigmy App:</b>
Facilitates pigmy collectors in collecting deposits and handling customer loans.<br>
<b>9. NEFT App: </b>
The app allows any member of the public to transfer funds directly to the accounts of society members.<br>
<b>Inward :</b> Society receives Money from the public.<br>
<b>Outward:</b> Money transferred out of the society. Society members can initiate outward transfers or drafts. Approval of outward drafts or transactions can be managed by organization staff. 

<b>10. Ais center App:</b>
Core banking system controlled by Ais center app and which is used by Automation staff.
