::: mermaid
 graph TD;
 Cust[Customer] -->MRK[Marketing Section];
MRK-->GP([Get preliminary details  <br>commitments on data as per data <br>conversion pre-requisites from mrk]) ;
GP-->SS[Support Section];
SS-->DC(["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px>Data Conversion Process</span>"]);
Dev[Development]-->A([Assist for technical<br> assistance required])
A-->DC;
MRK-->DT([Date and time should be given to<br> the customer after confirmation<br> from Support/deployment manager]);


click DC
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/145/Data-Conversion-Process"
:::
