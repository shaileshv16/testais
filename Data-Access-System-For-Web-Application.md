::: mermaid
 graph TD; 
A[(<b> SahakariDBAll)];
B[(<b> SmartfinAuthDB)];
C[(<b> BirseAuthDB<br> Postgres)];
D[(<b> Microsoft Entra)];
A-->|Authentication| E[<b> Sahakari App];
B-->|Authentication| F[<b> Smart BC];
B-->|Authentication| G[<b> Smart Fincore];
B-->|Authentication| H[<b> Smart Community App];
B-->|Authentication| I[<b> Birse Finserve];
C-->|Authentication| J[<b> Birse CRM];
D-->|Authentication| K[<b> Birse Smart Mobile App];
E-->|Org-Data| L(<b> CenterAuth<br>authconnect.dll);
F-->|Org-Data| L(<b> CenterAuth<br>authconnect.dll);
G-->|Org-Data| L(<b> CenterAuth<br>authconnect.dll);
H-->|Org-Data| L(<b> CenterAuth<br>authconnect.dll);
I-->|Org-Data| L(<b> CenterAuth<br>authconnect.dll);

K-->|Org-Data| L(<b> CenterAuth<br>authconnect.dll);

A-->|Few Data| E;
F-->|Dashboard Data|A;
J-->|Org-Data| N[(<b>PostgreSQL)];
J-->|Org-Data| L;
subgraph Databases
A1[(<b>Databases)]
A2[(<b>Databases)];
A3[(<b>Databases)];
end
L-->|Connection String| A2;
style A fill:#f8eab1  , stroke:#030002  , stroke-width:3px;
style B fill:#ebf8b1  , stroke:#030002  , stroke-width:3px;
style C fill:#c8f8b1  , stroke:#030002  , stroke-width:3px;
style D fill:#b1f8d9  , stroke:#030002  , stroke-width:3px;
style E fill:#eef8b1  , stroke:#030002  , stroke-width:3px;
style F fill:#ead8fe  , stroke:#030002  , stroke-width:3px;
style G fill:#d8fef5  , stroke:#030002  , stroke-width:3px;
style H fill:#d1a3f8   , stroke:#030002  , stroke-width:3px;
style I fill:#ffcac8 , stroke:#030002  , stroke-width:3px;
style J fill:#d8edfe  , stroke:#030002  , stroke-width:3px;
style K fill:#d2fca0   , stroke:#030002  , stroke-width:3px;
style L fill:#f6d8fe  , stroke:#030002  , stroke-width:3px;
style N fill:#f1eaf3  , stroke:#030002  , stroke-width:3px;
style A1 fill:#a3b6f8   , stroke:#030002  , stroke-width:3px;
style A2 fill:#a3b6f8   , stroke:#030002  , stroke-width:3px;
style A3 fill:#a3b6f8   , stroke:#030002  , stroke-width:3px;


:::
<br>
<br>

This diagram represents an authentication and data flow structure across multiple applications and databases, Here’s a detailed breakdown:<br>
<b>Sahakari DB all:</b> This seems to be a database that serves the Sahakari App for authentication purposes.<br>
<b>Smart fin auth DB:</b> This database handles authentication for several applications related to "Smart" branded services (e.g., Smart Fincore, Smart BC, Smart Community App, Birse Finserve).<br>
<b>Birse auth DB (Postgres):</b> A PostgreSQL database used specifically for authenticating Birse CRM.<br>
<b>Microsoft Entra:</b> This is an identity and access management solution (likely from Microsoft's Entra platform), which handles authentication for Birse Smart Mobile App.

 Apps utilizes the Center Auth as a bridge to access real data .
