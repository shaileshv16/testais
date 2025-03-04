::: mermaid
 graph TD;
 A([Amount deposited in<br> Yes Bank/SBI]) --> AC[Accounts];
AC-->UGS([Update in ACSPL <br>GST google sheet]);
UGS-->AR{If<br> Amount received<br> to yes bank};
AR-->|Yes| VGA([Voucher get generated<br> automatically]);
AR-->|No| GV([Generate the Voucher]);
GV-->PIR([Prepare the invoice by renewing<br> the dependent google sheet files]); 
PIR-->SIV([Send the invoice and voucher to the<br> customer through sales mail and <br> cc to reseller and MCP mail]);
SIV-->I([Update the information in <br> respective google sheet files]);
:::
