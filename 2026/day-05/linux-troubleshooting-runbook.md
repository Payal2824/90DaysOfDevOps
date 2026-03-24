# linux troubleshooting

##Environment : tell about the machine which is path,id,destination like where am I ?

uname -a ,lsb_release -a

1. check running process :- ps -o pid,pcpu,pmem,comm  -p $(pgrep Xorg | head -1)
2. memory usage :- free -h
3. disk usgae :- df -h
4. log directory size :- du -sh /var/log
5. ssh running and service check correctly listen :- ss -tulpn | grep ssh
6. connectivity test :- ping -c 3 localhost
7. service log :- journalctl -u ssh -n 50
8. system log :- tail -n 50 /var/loog/syslog


   if troubleshooting is happening and you check
   1. ssh service is running normally
   2. no CPU or memory spikes
   3. disk usage us within safe limits
   4. no suspicious error in log
   5. network connectivity is fine

   this evrything is fine then you check
   1. Restart services :- sudo systemctl restart.ssh
   2. increase logging and debug :- sudo journalctl -u ssh -f
   3. deep inspection :- sudo strace -p <pid>

