# centos
stuff about centos installation and admin

# samba issues
https://www.reddit.com/r/CentOS/comments/f1qf4o/centos_7_samba_not_working/

# docker issues
dns may not work, should try this: 
1/ 
> cat /etc/resolv.conf
Let's suppose it is 192.168.1.1, then put dns server address into /etc/default/docker
> DOCKER_OPTS="--dns 192.168.1.1"
2/ or this: 
> firewall-cmd --permanent --zone=trusted --add-interface=docker0
> firewall-cmd --reload
