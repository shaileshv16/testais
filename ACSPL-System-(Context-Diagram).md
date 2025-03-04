::: mermaid
 graph TD;
Customer["Customer"] -- Revenue--> A["<span style='text-decoration: underline; text-decoration-color: Blue;' text-decoration-thickness: 25px;>Internal System</span>"]

click A
"https://dev.azure.com/smartfincore/ACS%20Project/_wiki/wikis/ACS-Project.wiki/105/Internal-Entities"

    A -- Mrk,sales,service --> Customer

    A -- Renumerations Payment --> B["Channel Partners , <br>Authorized Mrk/service provider"]

    A -- Product and services--> B

    A -- Payments --> C["Supplier/Service Provider"]

    C -- Product and services --> A
B--Mrk,sales,service-->Customer

:::




