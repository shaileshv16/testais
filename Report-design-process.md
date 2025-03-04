::: mermaid
 graph TD;
 DS[Development Section]

 OTD[Other than development<br> Section: Ac, etc.];

DS-->|Requirement| RR([Report requirement<br> through mail]);

OTD-->|Requirement| RR;

RR-->|Requirement| RDS[Report design section];

RDS-->|Requirement| SR([Study the requirement]);

SR-->|Requirement| PQ([Prepare query and report<br> layout in dev.in system]);
PQ-->|Report| CSB([Compare that with <br>the Smart Bank]);
CSB-->|Report| CWSB([Compare that with the<br> smart bank]);
CWSB-->|Report| AR([Add that reports to the project<br> and test that report<br> C1]);  
AR-->|Report| SR([Send the report to <br>the QA Team]);
SR-->|Report| TP(["<span style='text-decoration: underline; text-decoration-color: Blue;'>Testing Process</span>"]);
TP-->|Review| ATP([After testing process report designer<br> receives review from the QA team]);
ATP-->|Report| GFR([Generate the final report based <br>on the review]);
ATP-->|Review| RDS;
click TP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/110/Testing-Process"
:::

**Checklist**

**C1:**
1. Check the report name
2. Check the report format
3. Check the language
4. Value checking
5. Report status checking