# ELK
The variables line in logstash need to match with log imported into logstash. 
This squid file should be located in logstash/patterns/ path. 

Early, I found a standard script from internet, but a lot of log can't be parsed. Some variables are not matched: src_ip, my squid catched x-forwared-IP, this is not single IP address, but ip strings, and some client includes ports, and sometines can't receive IP, instead of '-'; server_ip_or_peer_name sometime is '-'; mime_content_type sometimes is '-'.

My script revised these variables.
