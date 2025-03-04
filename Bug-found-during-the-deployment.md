::: mermaid
 graph TD;
  Bugs[Bugs]-->SS[Support Section];
SS-->|Bugs| RBO([Review the bug<br> observation]);
RBO-->|Bug details| ADT([Assignment to <br>development team]);
ADT-->|Bug details| Scrum[Scrum];
Scrum-->|Bug details| GBL([Get the bug list assign with <br> priority and get it done]);

GBL-->|Product| RPDN([Release the product <br> with deployment note]);
RPDN-->|Product released with <br>deployment documents| SS1[Support Section];
SS1-->DUC([Deployment and update <br> to the Customer]);
:::
