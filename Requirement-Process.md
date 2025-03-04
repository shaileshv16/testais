::: mermaid
 graph TD;
 Cust[Customer] -->|Requirement| ST[Support Team];
ST-->|Requirement| RAT[RAT];
SP[Service Provider]-->|Requirement| RAT;
MRK[MRK]-->|Requirement| RAT;
MNG[Management]-->|Requirement| RAT;
RAT-->|Requirement| RMR([RAT meeting to accept or<br> reject and prioritize the requirements<br>C1]);
 DEV[Development]--> |Assistance| RMR;
RMR--> |Check| IR{If <br>rejected?};
IR-->|Yes| IC([Intimations to customer/<br>Manager/MRK]);
IC-->END([End]);
IR-->|No| GE([Get effort estimations]);
DEV-->GE;
GE-->FR([Finalize the requirement <br>prioritize list]);
FR-->|Assignment list| Scrum[Scrum];
Scrum-->SDP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Software Development Process</span>"]);
SDP-->Devo[Developers];
click SDP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/140/Software-Development-Process"
:::

**Checklist**

**C1:**
1. Complexity of the project
2. Functional and non functional requirements
3. Is the requirement applicable to all customers or not?
4. Gather All Requirements
5. Review Requirements in Advance
6. Define Evaluation Criteria
7. Schedule the Meeting
8. Review Each Requirement
9. Evaluate Against Criteria
10. Decision Making
11. Document Decisions
12. Assign Ownership
13. Communicate Outcomes
14. Update Documentation
15. Follow-Up