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

curl -s http://example.com -w ' <br>
%{time_namelookup} <br>
%{time_connect} <br>
%{time_appconnect} <br>
%{%time_pretransfer} <br>
%{time_redirect} <br>
%{%time_starttransfer} <br>
%{time_total}' <br>
