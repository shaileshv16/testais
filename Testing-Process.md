::: mermaid
 graph TD;
 QAT[QA Team];
DP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>From Development Process</span>"])-->QAT;
RD(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>From Report Design</span>"])-->QAT;
QAT-->TR([Test the requirement based on<br> different test scenarios<br> C1]);
TR-->|Requirement| CR([Compare the requirement]);
CR-->|Requirement| UD([Upload reviews with<br> video through devops]);

click DP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/140/Software-Development-Process"

click RD
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/130/Report-design-process"
:::
