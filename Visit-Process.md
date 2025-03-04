::: mermaid
 graph TD;
 DM[Deployment Manager]
VR(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>From Visit Request</span>"])-->DM;
OP(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>From Order Process</span>"])-->DM;
DM-->|Check| SDO{Is <br>solution will<br> be done <br>through online?};
SDO-->|Yes| RT([A request ticket is<br> raised in  birse and <br>implemented in online]);
SDO-->|No| SV([Scheduling the visit<br> based on the availability of <br>customer and service person]);
SV-->|Visit assignment| SP[Service Person];
SP-->|Visit| VCF([Visit the customer and<br> receives feedback]);
click VR
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/109/Visit-Request"

click OP
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/134/Order-Process"
:::
