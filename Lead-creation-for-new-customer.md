::: mermaid
 graph TD;
 Mng[Management] -->|Lead creation target| MRK[MRK head];
MRK-->|Assignment| BDM[Business Development Manager];
 BDM-->MT[MRK team];
MT-->|Lead| SP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Sales Order Process</span>"]);
BDM-->| Lead & Plan| ET[External team];
ET-->|Intimation| MT;

Cus[Customer]
Cus--> |Lead reference| IT[ Inhouse team];

IT-->I([Inhouse lead Intimation<br>C1]);
I-->|Intimation| BDM;
R[Referral]-->|Lead intimation| BDM;
click SP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/147/Sales-Order-Process"
:::

**Checklist**

**C1:**
1. Various types of lead creation: Call, Visit, Seminars, Advertisement, Referral
2. Lead created source reference
3. Update the detail to the mrk lead files
4. Update the referral details in business detail file
5. Ensure the follow up done for positive leads

