#Curl Example



curl -s -w ' 
Namelookup: %{time_namelookup}
Connect: %{time_connect}
AppConnect: %{time_appconnect}
Pretransfer: %{%time_pretransfer}
Redirect: %{time_redirect}
StartTransfer: {%time_starttransfer}
----------------------------------
Total: %{time_total}' 

curl -s http://example.com -w ' 
%{time_namelookup}
%{time_connect}
%{time_appconnect}
%{%time_pretransfer}
%{time_redirect}
{%time_starttransfer}
%{time_total}' 
