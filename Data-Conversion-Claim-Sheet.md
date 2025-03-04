::: mermaid
 graph TD;
DCP(["<span style='text-decoration: underline; text-decoration-color: Blue;'>From Data Conversion Process</span>"])-->DCT;
 DCT[Data Conversion Team] -->|Claim sheet and<br> Approval sheet| DCM[Data Conversion Manager];
DCM-->|Check| C{If <br>both sheets reach the <br>same requirement}
C-->|Yes| A([Approve and send to the CSM]);
C-->|No| DCT;
A-->CSM[Customer Support Manager];
CSM-->|Check| C1{If <br>both sheets reach the <br>same requirement}
C1-->|Yes| A2([Approve and send to the Finance]);
C1-->|No| DCM;
A2-->Fin[Finance]
Fin-->|Check| A3{If <br>both sheets reach the <br>same requirement}
A3-->|Yes| A4([Process the Payment and<br> sanction ammount])
A3-->|No| CSM
:::
