# CURL
Curl examples

curl -s -w ' 

Namelookup: %{time_namelookup} <br>
Connect: %{time_connect} <br>
AppConnect: %{time_appconnect} <br> 
Pretransfer: %{%time_pretransfer} <br>
Redirect: %{time_redirect} <br>
StartTransfer: {%time_starttransfer} <br>

----------------------------------

Total: %{time_total}' 

curl -s http://example.com -w ' 
%{time_namelookup}
%{time_connect}
%{time_appconnect}
%{%time_pretransfer}
%{time_redirect}
%{%time_starttransfer}
%{time_total}' 
