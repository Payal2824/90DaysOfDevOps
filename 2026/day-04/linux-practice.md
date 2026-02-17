######Process and services#####

Process :-

ps aux | head -10 :- show running process but only show first 10 process beacause of head -10

top :- show running process , disk usage , CPU usage , Storage , load average

Service :-

systemctl status docker :- it will be system status active or not 
if docker is not found then installed it


systemctl list-unit --tupe=service --state=running :- list running services

journalctl -u docker --no-pager | tail -n 10 :- check log for doker services

mini troubleshooting are there :

application is not installed so , first installed it and same as command particular command run with sudo because root user permission is requied .
