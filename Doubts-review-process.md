::: mermaid
 graph TD;
 SE[Support Executives] -->|Doubts list| MRD([Mail regarding the doubts]);
MRD-->|Doubts list| TT[Technical Trainer];
TT-->|Doubts list| DTD([Decides the topic on  <br>maximum requested doubt]);
DTD-->|Doubts list| PD([Prepare document regarding<br> the selected topic]);
PD-->|Doubts list| SDT([Schedule the date and<br> time for the task]);
SDT-->|Date and Time| ISD([Inform the scheduled date and <br>time to the support executives]);
ISD-->|Date and Time| PT([Provides training to the<br> support executives on the<br> selected topic]);
PT-->|Training| ACT([After completing the training<br> prepare for the test <br> C1]);
ACT-->|Test| CK([Conducting a knowledge test for<br> the support executives to <br>assess their understanding]);
ISD-->SE;
:::
