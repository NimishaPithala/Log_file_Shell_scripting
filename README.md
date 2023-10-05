# Log_file_Shell_scripting
This assignment is in collaboration with BTH University.

shell scripts were written to read a log file and answers the following
questions:
• Which IP addresses makes the most number of connection attempts?
• Which IP addresses makes the most number of successful connection
attempts?
• What are the most common result codes and where do they come from
(IP number)?
• What are the most common result codes that indicate failure (no auth,
not found etc) and where do they come from?
• Which IP number get the most bytes sent to them?



The output format should be in the form:
-c: xxx.xxx.xxx.xxx yyy where yyy is the number of connection attempts
-2: xxx.xxx.xxx.xxx yyy where yyy is the number of successful attempts
-r: yyy xxx.xxx.xxx.xxx where yyy is the result code, one ip per line
-F: yyy xxx.xxx.xxx.xxx where yyy is the result code indicating failure,
one ip per line
-t: xxx.xxx.xxx.xxx yyy where yyy is the number of bytes sent from
the server
where -c -2 -r -F -t are the commands.

Additional Task was,
to get the DNS name associated with each IP number and then double check that DNS name against the DNS blacklist available at the course page (filename is dns.blacklist.txt). This feature should be available as argument -e in the scripts argument list and it should be possible to use -e in combination with other arguments ’(-c|-2|-r|-F|-t)’. If argument -e is specified all DNS names (related to the IPs in the log) should be compared with each entry in the blacklist. If a match is found, then the
end of the output of such a line output should be Blacklisted". Otherwise, no additional output is needed.

(Taken from the assignment document provided by the BTH University)
